---
title: "Serving Agentic Workloads at Scale with vLLM x Mooncake"
type: application
research_topic: "AI 應用與部署 / AI Applications & Deployment"
date_published: "2026-05-06"
date_collected: "2026-07-14"
date_updated: "2026-07-14"
source_url: "https://vllm.ai/blog/2026-05-06-mooncake-store"
identifier: "vllm-mooncake-agentic-workloads-2026"
tags:
  - ai
  - application
  - llm
  - inference
  - optimization
  - deployment
  - vllm
---

# Serving Agentic Workloads at Scale with vLLM x Mooncake

## 概述

vLLM 與 Mooncake Store 整合分散式 KV cache pool，針對長時間、多輪工具調用的 agentic workloads，降低重複計算大型共用前綴所造成的推論成本。

這項設計讓多個 vLLM instance 共用叢集層級的 KV cache，避免工作階段被路由至不同 instance 時重新計算相同前綴。

## 工作負載特徵

官方文章分析 Codex 與 SWE-bench Pro 的 agentic traces，指出這類工作負載具有：

- 長時間、多輪互動
- 每輪重複使用大量既有前綴
- 新增 token 相對少
- input-to-output token ratio 約為 131:1
- context 可由約 12K 成長至 80K tokens，最長超過 180K tokens

因此，傳統只依賴單一 instance 本機 KV cache 的架構容易遭遇容量不足與跨 instance cache miss。

## 架構設計

Mooncake Store 提供叢集層級的分散式 KV cache pool：

- Mooncake master 管理 KV block metadata、服務探索與節點健康狀態
- 各 GPU node 執行 Mooncake client
- 使用 RDMA 在 GPU HBM、CPU DRAM 或其他節點間移動 KV blocks
- 透過 GPUDirect RDMA 進行零拷貝傳輸
- 使用背景 I/O thread，避免阻塞主要推論路徑
- 透過 vLLM KVConnector 與 MultiConnector 整合

## 官方測試結果

在官方 Codex agentic trace 測試中，使用 1P1D 與 12 張 GB200 GPU：

- 吞吐量提升 3.8 倍
- P50 TTFT 降低 46 倍
- 端到端延遲降低 8.6 倍
- cache hit rate 從 1.7% 提升至 92.2%

在擴展測試中：

- GPU 數量由 12 張擴展至 60 張
- cache hit rate 維持在 95% 以上
- 整體吞吐接近線性擴展

以上數據只適用於官方測試環境與指定工作負載，不應直接推廣至所有模型與部署情境。

## 核心價值

對具有大量重複前綴的多輪代理人工作負載而言，分散式 KV cache 能降低跨 instance 路由造成的重算成本，並提升叢集資源共享效率。

其價值不只是單一模型推論加速，而是將 KV cache 從 instance 本機資源提升為叢集層級的共享基礎設施。

## 應用情境與實務影響

- 程式開發代理人
- 長時間多輪工具調用工作流
- 大型共享 system prompt
- 多租戶代理人平台
- 跨節點 LLM serving
- Prefill-decode disaggregation 架構
- 大規模 GPU 叢集的 KV cache 管理

## 部署限制與注意事項

- 官方結果使用 GB200 GPU，其他硬體不能直接套用相同數字。
- 效益高度依賴前綴重複率與 cache hit rate。
- RDMA 與 GPUDirect RDMA 會增加網路與基礎設施要求。
- 分散式 cache metadata、節點故障與資料一致性需要額外治理。
- 官方實作仍在持續開發，部分功能列於後續規劃。
- 實際部署應以自身模型、context 長度、路由方式與流量分布重新 benchmark。

## 來源

- 官方文章：https://vllm.ai/blog/2026-05-06-mooncake-store
- Mooncake Repository：https://github.com/kvcache-ai/Mooncake

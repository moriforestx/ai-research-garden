---
title: "SuperInfer: SLO-Aware Rotary Scheduling and Memory Management for LLM Inference on Superchips"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-05-19"
organization: "MLSys 2026"
source_url: "https://proceedings.mlsys.org/paper_files/paper/2026/hash/07fd64f9316f40193c6a4d87d8afa011-Abstract-Conference.html"
date_collected: "2026-09-24"
date_updated: "2026-09-24"
tags:
  - ai
  - paper
---

# SuperInfer: SLO-Aware Rotary Scheduling and Memory Management for LLM Inference on Superchips

## 基本資訊

- 發布日期：2026-05-19
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://proceedings.mlsys.org/paper_files/paper/2026/hash/07fd64f9316f40193c6a4d87d8afa011-Abstract-Conference.html

## 概要

提出 SuperInfer，一種專為新世代 Superchips（如 NVIDIA GH200）設計的高效能 LLM 推理系統，透過 SLO-aware 旋轉排程器（RotaSched）和高效能旋轉引擎（DuplexKV）解決長請求序列下的 KV cache 耗盡與 head-of-line 阻塞問題。RotaSched 主動輪調請求以維持 Superchips 上的響應性，而 DuplexKV 則實現 NVLink-C2C 上的全雙工傳輸，顯著提升 Time-To-First-Token (TTFT) 服務水準目標 (SLO) 達成率。

## 核心價值

首次提出針對服務水準目標 (SLO) 的主動排程策略於 LLM 推理系統中，結合記憶體與運算的共同設計，充分釋放異構 Superchips 在響應性 LLM 服務中的潛力，突破傳統被動調度的瓶頸。

## 應用情境與實務影響

適用於需要低延遲和高吞吐量的 LLM 服務場景：對話式 AI、程式設計夥伴、即時翻譯等；在相同硬件條件下提升服務容量或降低基礎設施成本；使企業級 LLM 部署更具可預測性與成本效益。

## 補充細節

論文於 2026-05-19 在 MLSys 2026 會議上發表。SuperInfer 針對 LLM 推理中兩個核心張力：嚴格的延遲服務水準目標 (SLO) 與有限的 GPU 記憶體容量。當高請求率耗盡 KV cache 預算時，傳統推理系統常嚴重頭部阻塞 (HOL) 導致 TTFT 和 TBT SLO 未達標。SuperInfer 的創新包括：(1) RotaSched：首個主動、SLO-aware 的旋轉排程器，根據服務水準目標動態輪調請求以維持系統響應性；(2) DuplexKV：高效能旋轉引擎，利用 NVLink-C2C 實現全雙工傳輸，減少記憶體搬運開銷。在 NVIDIA GH200 Superchip 上使用各種模型和資料集進行評估，結果顯示：相比現有 SOTA 系統，SuperInfer 使 TTFT SLO 達成率提升高達 74.7%，同時保持相当的 TBT (Time-Between-Token) 和吞吐量。此工作为突破 LLM 推理系統的擴展瓶頸提供了創新解決方案，特別是對於需要即時回應的生產環境具有重要價值。代碼已作為 vLLM v0.6.6.post1 的 fork 提供，便於社區採用與延伸。

## 維護紀錄

- 收錄日期：2026-09-24
- 最後更新：2026-09-24

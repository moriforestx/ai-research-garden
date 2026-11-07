---
title: "OpScale: Operator-level Provisioning and Autoscaling for LLM Serving"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-08-14"
organization: "Microsoft Research"
source_url: "https://arxiv.org/abs/2608.13499"
date_collected: "2026-11-08"
date_updated: "2026-11-08"
tags:
  - ai
  - paper
---

# OpScale: Operator-level Provisioning and Autoscaling for LLM Serving

## 基本資訊

- 發布日期：2026-08-14
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2608.13499

## 概要

Microsoft Research 提出 OpScale，首個運算元級別的 LLM 推理編排框架，解決「縮放單位應為何」的根本問題。傳向將整個模型視為單體縮放單位，忽略運算元異質性；OpScale 以運算元 DAG 為基礎，執行剖析、佈署、放置與運行時服務四階段，在生產流量追蹤下於 40 張 A100 與 24 張 GB200 上驗證，達到 SLO 同時降低成本高達 36.3%。原型建於 nano-vLLM 之上（約 17K 行 Python），繼承 PagedAttention、連續批次、張量並行等關鍵優化。

## 核心價值

重新定義 LLM 服務縮放顆粒度，從模型級下探至運算元級，證明細粒度彈性能顯著提升 GPU 叢集成本效益。

## 應用情境與實務影響

雲端 GPU 集群運營商、大規模 LLM 服務提供商可直接採用 OpScale 邏輯重構自動縮放器；開源實作預期釋出，可整合進 vLLM、SGLang 等主流服務框架。

## 補充細節

論文編號 arXiv:2608.13499v1，分類 cs.DC、cs.AI。作者來自 Microsoft Research。實驗模型涵蓋 Qwen2-7B、Llama3-8B、Qwen2.5-VL-32B（密集）與 Qwen2-MoE、Mixtral-8x7B（MoE）。核心發現：運算元間計算強度、記憶體壓力、並行度差異巨大，單體縮放導致資源碎片化；OpScale 的運算元級佈署與放置算法在生產追蹤下平均省 20-36% 成本。

## 維護紀錄

- 收錄日期：2026-11-08
- 最後更新：2026-11-08

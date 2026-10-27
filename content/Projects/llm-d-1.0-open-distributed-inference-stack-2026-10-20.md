---
title: "llm-d 1.0: 開源分布式 LLM 推理堆疊達到生產就緒里程碑"
type: project
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-20"
organization: "llm-d Project (CNCF Sandbox), Google, Red Hat, IBM, NVIDIA, CoreWeave"
source_url: "https://cloud.google.com/blog/topics/ai-infrastructure/llm-d-1-0-an-open-source-stack-for-distributed-inference"
date_collected: "2026-10-28"
date_updated: "2026-10-28"
tags:
  - ai
  - project
---

# llm-d 1.0: 開源分布式 LLM 推理堆疊達到生產就緒里程碑

## 基本資訊

- 發布日期：2026-10-20
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://cloud.google.com/blog/topics/ai-infrastructure/llm-d-1-0-an-open-source-stack-for-distributed-inference

## 概要

llm-d 專案（CNCF Sandbox 專案）發布 v1.0 版，標誌著開源分布式 LLM 推理堆疊達到生產就緒成熟度。由 Google、Red Hat、IBM、NVIDIA、CoreWeave 共同創立，超過 500 位貢獻者、25+ 組織參與。整合 vLLM、SGLang 推理引擎與 Kubernetes 原生調度，提供前綴感知路由、KV 快取卸載、預填/解碼解耦、多租戶流量控制、無停機升級等 Day 2 運營能力。在 Ironwood TPU 上實測：代理編碼工作負載 TTFT 中位數降低 85% 以上、吞吐量提升 2.4 倍；上下文密集型代理工作負載成本降低 5-10 倍、輸出吞吐量提升 3 倍。

## 核心價值

確立了「任何模型、任何加速器、任何雲」的分布式推理開放標準，填補 vLLM/SGLang 單節點高效但缺乏生產級分布式編排的關鍵缺口。

## 應用情境與實務影響

企業可直接採用 llm-d 1.0 在 GKE、AKS、EKS、CoreWeave、OpenShift 等任意 Kubernetes 環境部署生產級 LLM 推理服務，支援多模型多租戶、SLA 保證、成本優化，顯著降低代理式應用的推理基礎設施門檻。

## 補充細節

發布日期 2026-10-20（PyTorch Conference 同步發布）。Google Cloud 部落格：https://cloud.google.com/blog/topics/ai-infrastructure/llm-d-1-0-an-open-source-stack-for-distributed-inference；IBM 新聞稿：https://newsroom.ibm.com/2026-10-20-llm-d-1-0-advances-open,-cost-efficient-ai-inference-for-production-scale；官方專案：https://llm-d.ai（v1.0 部落格文章）。創始組織：Red Hat、IBM、Google Cloud、CoreWeave、NVIDIA；支援加速器：NVIDIA GPU、Google TPU、AMD GPU、Intel Gaudi；推理引擎：vLLM、SGLang。

## 維護紀錄

- 收錄日期：2026-10-28
- 最後更新：2026-10-28

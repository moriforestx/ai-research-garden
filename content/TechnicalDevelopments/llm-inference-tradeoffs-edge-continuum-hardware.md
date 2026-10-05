---
title: "A Measurement Study of LLM Inference Trade-offs Across Edge Continuum Hardware"
type: technical-development
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-08"
organization: "學術研究團隊"
source_url: "https://arxiv.org/abs/2609.08307"
date_collected: "2026-10-06"
date_updated: "2026-10-06"
tags:
  - ai
  - technical-development
---

# A Measurement Study of LLM Inference Trade-offs Across Edge Continuum Hardware

## 基本資訊

- 發布日期：2026-09-08
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.08307

## 概要

針對邊緣到近邊緣部署節點（NVIDIA Jetson AGX Orin、CPU/GPU 伺服器）的受控量測研究，評估多個開放權重 LLM 及量化變體在品質、延遲、模型大小與能耗間的權衡。涵蓋 Orca、vLLM、Sarathi-Serve 等服務系統，並對比量化方法對推理效率的影響。

## 核心價值

提供跨硬體層級的實證基準，量化邊緣部署中模型品質、延遲、記憶體佔用與能耗的具體折線關係。

## 應用情境與實務影響

指導邊緣 AI 應用選型：在給定硬體預算下平衡模型精度與服務品質，降低自架推理的試錯成本。

## 補充細節

arXiv:2609.08307v1，2026-09-08 提交。屬 cs.DC（分散式、平行與叢集運算）類別。實驗平台包含 Jetson AGX Orin（邊緣）與雙路 CPU/GPU 伺服器（近邊緣）。評估模型涵蓋 Llama、Qwen、Mistral 等開放權重家族及其 INT4/GPTQ/AWQ 量化版本。

## 維護紀錄

- 收錄日期：2026-10-06
- 最後更新：2026-10-06

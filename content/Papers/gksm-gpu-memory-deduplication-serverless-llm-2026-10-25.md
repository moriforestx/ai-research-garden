---
title: "gKSM：驅動層 GPU 記憶體去重，釋放無伺服器 LLM 推理叢集容量"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-25"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2610.25219"
date_collected: "2026-10-26"
date_updated: "2026-10-26"
tags:
  - ai
  - paper
---

# gKSM：驅動層 GPU 記憶體去重，釋放無伺服器 LLM 推理叢集容量

## 基本資訊

- 發布日期：2026-10-25
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2610.25219

## 概要

提出 gKSM，在 GPU 驅動層實現跨推理框架（vLLM、SGLang、TensorRT-LLM）的記憶體去重。解決現有策略僅能去重完全相同模型實例、無法跨框架共享、無法利用微調模型間部分權重共享三大限制。實驗顯示去重節省的記憶體可直接轉化為更高叢集容量，提升無伺服器 LLM 推理的成本效益。

## 核心價值

首創驅動層跨框架記憶體去重，打破推理引擎孤島，支援不同框架、不同微調模型間的細粒度權重共享。

## 應用情境與實務影響

降低 LLM 推理服務的 GPU 記憶體壓力，提升無伺服器部署密度與成本效率；為雲端供應商與自建推理平台提供通用優化路徑。

## 補充細節

對比 vLLM（55% 採用率）、TensorRT-LLM（45%）、SGLang（30 萬+ GPU 部署）三大生態。實驗模型涵蓋 Qwen3-8B、Qwen2.5-7B、GLM-4-9B、Llama3-8B 及其指令微調版本。主題：cs.DC、cs.OS。

## 維護紀錄

- 收錄日期：2026-10-26
- 最後更新：2026-10-26

---
title: "ProEval: Proactive Failure Discovery and Efficient Performance Estimation for Generative AI Evaluation"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-04-25"
organization: "Google DeepMind"
source_url: "https://deepmind.google/research/publications/238239"
date_collected: "2026-08-12"
date_updated: "2026-08-12"
tags:
  - ai
  - paper
---

# ProEval: Proactive Failure Discovery and Efficient Performance Estimation for Generative AI Evaluation

## 基本資訊

- 發布日期：2026-04-25
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://deepmind.google/research/publications/238239

## 概要

Google DeepMind 提出 ProEval，一個針對生成式 AI 評估的主動評估框架。利用預訓練高斯過程 (GP) 作為效能分數函數的代理模型，透過遷移學習跨基準泛化，在嚴格評估預算下以 8–65 倍更少樣本達到 ±1% 地面真值準確度，同時主動發現更多樣化的失效案例。於 GSM8K、MMLU、StrategyQA、Jigsaw 等推理、安全與分類基準驗證。ICML 2026 入選，代碼與數據開源 (Apache 2.0 / CC-BY)。

## 核心價值

以代理模型與遷移學習大幅降低 GenAI 評估成本（最多 100 倍），並從被動基準測試轉向主動失效發現，解決大模型評估昂貴、緩慢且難以全面覆蓋的痛點。

## 應用情境與實務影響

企業與研究者可在有限預算下全面評估模型推理、安全與分類能力，部署前主動發現邊緣失效案例，顯著降低生產環境風險。

## 補充細節

作者：Yizheng Huang、Wenjun Zeng、Aditi Kumaresan、Zi Wang (Google DeepMind)。arXiv：2604.23099 (2026-04-24 提交)。ICML 2026 正式發表。GitHub：https://github.com/google-deepmind/proeval。DeepMind 發布頁：https://deepmind.google/research/publications/238239。

## 維護紀錄

- 收錄日期：2026-08-12
- 最後更新：2026-08-12

---
title: "Large Language Models Explore by Latent Distilling"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-04-24"
organization: "ICML 2026"
source_url: "https://arxiv.org/abs/2604.24927"
date_collected: "2026-10-19"
date_updated: "2026-10-19"
tags:
  - ai
  - paper
---

# Large Language Models Explore by Latent Distilling

## 基本資訊

- 發布日期：2026-04-24
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2604.24927

## 概要

提出 Exploratory Sampling (ESamp) 解碼方法，透過線上 Latent Distiller (LD) 將淺層表示映射至深層表示，以預測生成軌跡的新穎度，引導 LLM 產生語義多樣而非表層變體的回應。論文於 ICML 2026 發表，解決測試時擴展中語義冗餘問題，無需外部模型或額外推理通道即可實現語義級多樣性探索。

## 核心價值

首創在 LLM 內部「思考過程」直接操作的語義多樣性解碼，Latent Distiller 以淺層到深層表示映射的不可預測性作為新穎度代理，同時解決語義相似度測量、無外部依賴、記憶累積、直接調制下一詞預測四大挑戰。

## 應用情境與實務影響

為 LLM 推理階段多樣性生成提供輕量級即插即用方案；適用於需多樣候選的場景（程式碼生成、創意寫作、推理路徑探索）；無額外推理開銷，相容現有部署架構。

## 補充細節

arXiv:2604.24927，ICML 2026 Poster #63542。作者 Y. Zeng 等人。實驗顯示 ESamp 在多項基準上顯著提升語義多樣性且不降低生成品質；Latent Distiller 僅需淺層 MLP，參數量極小。

## 維護紀錄

- 收錄日期：2026-10-19
- 最後更新：2026-10-19

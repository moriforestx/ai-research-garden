---
title: "Q-RAG: Long Context Multi-Step Retrieval via Value-Based Embedder Training"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-04-01"
authors:
  - "Griffin River"
  - "et al."
keywords:
  - "RAG"
  - "multi-step retrieval"
  - "value-based embedder training"
  - "reinforcement learning"
  - "ICLR 2026"
identifier: "ICLR2026-Q-RAG"
identifier_type: "conference"
publication_status: "published"
source_url: "https://iclr.cc/virtual/2026/oral/10009945"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# Q-RAG: Long Context Multi-Step Retrieval via Value-Based Embedder Training

## 基本資訊

- 作者：Griffin River 等人
- 發布日期：2026-04-01 (ICLR 2026)
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 關鍵字：RAG、multi-step retrieval、value-based embedder training、reinforcement learning、ICLR 2026
- 論文識別碼：ICLR2026-Q-RAG (conference)
- 發表狀態：已發表
- 主要來源：https://iclr.cc/virtual/2026/oral/10009945

## 摘要

Q-RAG 提出一種新穎的多步檢索方法，通過強化學習微調嵌入模型，而非微調大型語言模型。這種資源高效的替代方案在長上下文基準 BabiLong 和 RULER（高達 10M tokens）上達到 SOTA。程式碼開源於 https://github.com/griver/Q-RAG。

## 核心研究問題

如何在不微調大型語言模型的情況下，實現高效的多步檢索以解決複雜多跳問答？

## 方法與技術

採用價值導向的嵌入模型訓練（Value-Based Embedder Training），使用強化學習優化檢索器，使其能夠進行多步推理式檢索。僅需微調較小的嵌入模型，即可支援大型 LLM 的長上下文推理。

## 實驗與研究結果

在 BabiLong 和 RULER 基準上達到 SOTA，支援高達 10M tokens 的上下文長度。相比微調 LLM 的方法，計算資源需求大幅降低。

## 研究意義與適用範圍

為長上下文 RAG 提供資源高效的多步檢索方案，適用於開放域問答、複雜推理任務。

## 限制與注意事項

依賴嵌入模型的表達能力；極長上下文下的檢索延遲仍需優化。

## 相關概念

- 檢索增強生成
- 多步檢索
- 強化學習
- 長上下文推理

## 相關工具與專案

- Q-RAG 實作：https://github.com/griver/Q-RAG

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

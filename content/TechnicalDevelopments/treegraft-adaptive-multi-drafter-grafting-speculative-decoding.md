---
title: "TreeGraft: Adaptive Multi-Drafter Grafting for Tree-Based Speculative Decoding"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-05-28"
organization: "多機構合作（作者單位未在摘要明確列出）"
source_url: "https://arxiv.org/abs/2608.26112"
date_collected: "2026-08-30"
date_updated: "2026-08-30"
tags:
  - ai
  - technical-development
---

# TreeGraft: Adaptive Multi-Drafter Grafting for Tree-Based Speculative Decoding

## 基本資訊

- 發布日期：2026-05-28
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2608.26112

## 概要

提出 TreeGraft，一個多草稿模型協作的樹狀投機式解碼框架。解決單一草稿模型在速度與品質間的兩難：小模型快但樹品質低、大模型品質好但延遲高。TreeGraft 讓不同成本的草稿模型共同構建草稿樹，強模型重新評分弱模型候選、重選嫁接位置、恢復未探索的優質路徑，並非破壞性整合強模型擴展。引入離線蒸餾的輕量調度器控制何時調用強模型。

## 核心價值

首個多草稿協作的樹狀投機解碼系統，在 10 組模型配對與 6 個基準上平均超越最佳單草稿策略 15.1%，最高達 26.6%，為 LLM 推理加速提供實用新范式。

## 應用情境與實務影響

直接適用於生產環境 LLM 服務推理加速，無需外部獎勵模型或標註資料；代碼開源於 https://anonymous.4open.science/r/TreeGraft-E983

## 補充細節

arXiv:2608.26112v1，提交日期 2026-05-28；屬 cs.CL 領域。作者來自多機構合作。

## 維護紀錄

- 收錄日期：2026-08-30
- 最後更新：2026-08-30

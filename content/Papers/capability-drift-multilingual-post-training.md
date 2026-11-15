---
title: "獎勵函數之外：多語言後訓練中的能力漂移"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-11-16"
organization: "Independent / Academic"
source_url: "https://arxiv.org/html/2611.15717v1"
date_collected: "2026-11-16"
date_updated: "2026-11-16"
tags:
  - ai
  - paper
---

# 獎勵函數之外：多語言後訓練中的能力漂移

## 基本資訊

- 發布日期：2026-11-16
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/html/2611.15717v1

## 概要

論文系統研究多語言後訓練（SFT + RL）過程中，基準分數上升卻伴隨著目標語言能力、輸出慣例等使用者關鍵行為退化的現象。以 Indic 語言為例，經過三輪 RL 後，較早檢查點的抽取能力消失，但透過無獎勵的知識蒸餾（僅用教師模型 next-token 分布）可大幅恢復。基準評分機制在 2026-08 下旬變更，導致不同輪次凍結不同評分規則，需嚴格重新評分才能公平比較。

## 核心價值

揭示「基準分數提升 ≠ 實用能力保持」的根本張力；證明知識蒸餾無需任務獎勵即可挽回後訓練導致的能力漂移，為持續適應提供低成本修正路徑。

## 應用情境與實務影響

多語言產品部署需監控「隱性退化」；建立蒸餾回溯機制可在不重跑 RL 的情況下修正語言能力流失，降低維運成本。

## 補充細節

作者 Sutanshu Saksena Raj 等人；實驗模型為 RL-Indic 系列，三輪後訓練（SFT → RL-Base → RL-Indic）。關鍵發現：(1) 後期 RL 會抹除早期 SFT/RL 的語言特定增益；(2) 從早期檢查點蒸餾可恢復 80%+ 抽取能力；(3) 基準評分規則變更導致跨輪次比較失真，須統一重評。入選 NeurIPS 2026 Workshop「Foundations of LLM Post-Training in Changing Environments」。

## 維護紀錄

- 收錄日期：2026-11-16
- 最後更新：2026-11-16

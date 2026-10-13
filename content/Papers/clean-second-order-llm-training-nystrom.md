---
title: "Clean: Second-order LLM Training at Linear Memory Cost via Nyström Sketching"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-04"
organization: "N/A"
source_url: "https://arxiv.org/abs/2610.04204"
date_collected: "2026-10-14"
date_updated: "2026-10-14"
tags:
  - ai
  - paper
---

# Clean: Second-order LLM Training at Linear Memory Cost via Nyström Sketching

## 基本資訊

- 發布日期：2026-10-04
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2610.04204

## 概要

提出 Clean 優化器，利用 Nyström Sketching 在線性記憶體成本下實現二階 LLM 訓練。Clean 的優化器狀態記憶體佔用比 AdamW 更小，却能在 26% 更少的牆鐘時間內達到 AdamW 同等性能。進一步提出 Q-Clean 低精度版本，預訓練 LLaMA-1.3B 架構時優化器記憶體較 Muon 降低 50% 以上，且保持競爭性能。在 350M 至 1.3B 參數規模驗證，預條件器每 10 步刷新，秩 r=256/512。

## 核心價值

突破二階優化在 LLM 訓練中的記憶體瓶頸，證明線性記憶體二階方法可超越一階基線，為大規模訓練降本增效提供新範式。

## 應用情境與實務影響

LLM 預訓練加速、GPU 記憶體優化、訓練成本降低、大模型優化器設計參考。

## 補充細節

arXiv:2610.04204v2，提交於 2026-10-04。屬 cs.LG、cs.AI、cs.CL 跨領域。作者提出基於 Nyström Sketching 的低秩近似，將二階動量矩陣壓縮至線性記憶體；Q-Clean 進一步量化優化器狀態。實驗覆蓋 LLaMA 架構 350M/1.3B，對比 AdamW、Muon、ALSO 等基線。代碼與實驗細節見論文。

## 維護紀錄

- 收錄日期：2026-10-14
- 最後更新：2026-10-14

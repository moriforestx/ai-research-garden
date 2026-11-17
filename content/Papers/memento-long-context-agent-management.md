---
title: "MEMENTO: Learning Context Management for Long Context Processing Agents"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-30"
organization: "Columbia University"
source_url: "https://arxiv.org/abs/2611.00244"
date_collected: "2026-11-18"
date_updated: "2026-11-18"
tags:
  - ai
  - paper
---

# MEMENTO: Learning Context Management for Long Context Processing Agents

## 基本資訊

- 發布日期：2026-10-30
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2611.00244

## 概要

MEMENTO 是一個基於 Qwen3-8B 的長上下文代理，透過上下文壓縮學習管理上下文。研究發現現成代理模型（含 GPT-5.5、GLM-5.3）常撰寫無效筆記，且單純 RL 難發現有用的記筆行為。MEMENTO 先以合成軌跡微調啟動記筆能力，再用結合答案正確性、筆記品質啟發式、信心校準的獎勵進行 RL 強化。僅在 20K tokens 上下文窗口下，於四個書級問答基準（最長 2.5M tokens）將 Qwen3-8B 準確率從 36.9% 提升至 67.8%，超越同環境下的 GPT-5.5 agent (13.1%) 及全書上下文 (56.7%)，成本不足 1/50；亦接近 100x 更大的 GLM-5.3 agent (69.3%)，成本僅 1/9。

## 核心價值

證明小模型經過專門的上下文管理訓練，能以極低成本在長文本任務上媲美甚至超越超大模型，為長上下文代理架構提供新範式。

## 應用情境與實務影響

大幅降低長文本處理（法律文檔、代碼庫、書籍、醫療記錄）的計算成本；為資源受限環境部署長上下文代理提供可行路徑。

## 補充細節

提交日期：2026-10-30 (v1)。作者來自哥倫比亞大學（Kathleen McKeown 等）。代碼與實驗細節見論文。

## 維護紀錄

- 收錄日期：2026-11-18
- 最後更新：2026-11-18

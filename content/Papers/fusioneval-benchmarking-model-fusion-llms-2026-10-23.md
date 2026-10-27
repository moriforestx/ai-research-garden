---
title: "FusionEval: Benchmarking Model Fusion for Large Language Models"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-23"
organization: "Multiple institutions (authors from various affiliations)"
source_url: "https://arxiv.org/abs/2610.30162"
date_collected: "2026-10-28"
date_updated: "2026-10-28"
tags:
  - ai
  - paper
---

# FusionEval: Benchmarking Model Fusion for Large Language Models

## 基本資訊

- 發布日期：2026-10-23
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2610.30162

## 概要

提出 FusionEval 基準測試，系統性評估大語言模型融合方法的能力保留度與計算成本。構建基於 Qwen3 與 Llama 開源模型的五領域專家池（數學、代碼、科學推理、指令遵循、工具使用），在八個公共基準上統一協議比較免訓練與需訓練融合方法。實驗發現：免訓練融合雖能保留推理能力，但在工具使用上顯著退化；需訓練方法雖全面但計算開銷大。提供標準化專家池、資料存取規則與計算效率指標（執行時間、峰值 GPU 記憶體），填補模型融合評估長鏈推理與工具使用覆蓋不足的空白。

## 核心價值

為模型融合領域建立首個覆蓋長鏈推理與工具使用的標準化基準，揭示免訓練融合在工具使用上的系統性缺陷，指導實務選型。

## 應用情境與實務影響

企業與研究者可直接用 FusionEval 評估融合策略權衡；專家池與評估腳本開源，可加速模型合併、知識蒸餾、持續預訓練等下游應用的基準化比較。

## 補充細節

arXiv:2610.30162v1 [cs.CL, cs.AI]，提交日期 2026-10-23。作者：Shuo Cai、Yanggan Gu、Yuhang Liu、Su Lu、Yuanyi Wang、Yang Yu、Zhen Li、Zhitian Hou、Guanghao Zhu、Ming Li、Hongxia Yang。基礎模型：Qwen3、Llama 系列。五領域專家獨立訓練。八基準：MATH、GSM8K、HumanEval、MBPP、GPQA、MMLU、IFEval、BFCL。報告歸一化平均分、最差分、運行時間、峰值 GPU 記憶體。

## 維護紀錄

- 收錄日期：2026-10-28
- 最後更新：2026-10-28

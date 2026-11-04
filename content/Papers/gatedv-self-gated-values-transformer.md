---
title: "GatedV: Self-Gated Values for Transformer Language Models"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-11-01"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.02145"
date_collected: "2026-11-05"
date_updated: "2026-11-05"
tags:
  - ai
  - paper
---

# GatedV: Self-Gated Values for Transformer Language Models

## 基本資訊

- 發布日期：2026-11-01
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2611.02145

## 概要

提出 GatedV，一種簡單的注意力變體，僅在聚合前對 Value 矩陣應用 SiLU 激活函數，不引入額外可訓練參數。在匹配參數量、配對初始化、相等訓練 token 預算下評估。

## 核心價值

2.33M 參數模型將平均 held-out perplexity 從 59.1 降至 57.9 (2.0%)；26.16M 參數模型從 20.2 降至 19.7 (2.4%)，所有配對種子均改善。

## 應用情境與實務影響

證明僅針對 Value 的自我閘控即可在不增加參數量、不重設計注意力加權機制的前提下提升語言建模性能，易於整合進現有 Transformer 架構。

## 補充細節

作者：Li-Ming Yu、Hongyu Zhou。arXiv:2611.02145v1，2026-11-01 提交；v2 2026-11-03。主題：Computation and Language (cs.CL); Machine Learning (cs.LG)。代碼：https://github.com/yuliming1996/GatedV

## 維護紀錄

- 收錄日期：2026-11-05
- 最後更新：2026-11-05

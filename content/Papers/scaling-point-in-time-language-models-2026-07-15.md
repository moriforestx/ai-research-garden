---
title: "Scaling Point-in-Time Language Models"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-07-15"
organization: "Yale University / EPFL / NBER / AQR Capital"
source_url: "https://arxiv.org/abs/2607.11889"
date_collected: "2026-08-03"
date_updated: "2026-08-03"
tags:
  - ai
  - paper
---

# Scaling Point-in-Time Language Models

## 基本資訊

- 發布日期：2026-07-15
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2607.11889

## 概要

研究嚴格時間點限制的語言模型預訓練：僅使用截至特定日期的網頁文本訓練，消除「未來資訊洩漏」導致的前視偏差。將模型擴展至 40 億參數、1 兆 chronological filtered tokens (FineWeb)，建構 2013–2024 年月度检查点序列，推理與語言理解表現逼近 Gemma-3-4B 與 LLaMA-7B 等無時間限制模型，且經濟預測免受前視偏差影響。

## 核心價值

證明大規模時間點訓練不犧牲通用能力，為金融/社科回測、因果推論提供無洩漏的語言模型基礎設施。

## 應用情境與實務影響

解決 LLM 在時序預測、金融建模、政策評估中不可用的核心痛點；月度檢查點序列可直接作為時間感知嵌入基礎設施部署。

## 補充細節

arXiv:2607.11889v2，提交日期 2026-07-15 (v1) / 2026-07-16 (v2)。42 頁、23 圖。作者：Bryan Kelly (Yale/NBER)、Semyon Malamud (EPFL/SFI)、Johannes Schwab (EPFL)、Teng Andrea Xu (AQR)。同步發布為 NBER Working Paper No. 35247 (May 2026)。

## 維護紀錄

- 收錄日期：2026-08-03
- 最後更新：2026-08-03

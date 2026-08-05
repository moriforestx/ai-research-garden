---
title: "Best-of-N TTS Evaluation is Confounded by ASR Family Alignment"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-07-09"
organization: "ICML 2026 Workshop"
source_url: "https://arxiv.org/abs/2607.08256"
date_collected: "2026-08-06"
date_updated: "2026-08-06"
tags:
  - ai
  - paper
---

# Best-of-N TTS Evaluation is Confounded by ASR Family Alignment

## 基本資訊

- 發布日期：2026-07-09
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2607.08256

## 概要

揭示 Best-of-N (BoN) TTS 推論時評估存在系統性偏差：當驗證器 ASR 與評估器 ASR 來自同一模型家族時，WER 指標會虛報改進。實驗證實跨家族評估才能反映真實內容正確度，並提出「語音版 LLM-as-a-Judge 自我偏好」類比。

## 核心價值

首次量化 TTS 評估中的 ASR 家族一致性偏差，推翻單一 ASR 驗證的可信度，建立跨家族評估新標準。

## 應用情境與實務影響

TTS 系統開發者需採用多家族 ASR 交叉驗證（Whisper、wav2vec2、HuBERT 等）才能獲得可信的 BoN 改進量測，避免虛假 SOTA 宣稱。

## 補充細節

ICML 2026 Workshop on Machine Learning for Audio 接收論文。涵蓋 F5-TTS、CosyVoice 2、MaskGCT、Seed-TTS、NaturalSpeech 3 等主流流匹配 TTS 系統。實驗證據排除音訊編碼器表示相似度（CKA）為主因，確認為模型血緣/身分層級耦合。

## 維護紀錄

- 收錄日期：2026-08-06
- 最後更新：2026-08-06

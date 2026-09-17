---
title: "StepAudio 3 Gen：統一語音與泛音頻生成的離散自迴歸模型"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-09-11"
organization: "StepAudio LLM Team"
source_url: "https://arxiv.org/abs/2609.12945"
date_collected: "2026-09-17"
date_updated: "2026-09-17"
tags:
  - ai
  - paper
---

# StepAudio 3 Gen：統一語音與泛音頻生成的離散自迴歸模型

## 基本資訊

- 發布日期：2026-09-11
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2609.12945

## 概要

StepAudio 3 Gen 為統一的泛音頻生成模型，支援零樣本 TTS、聲音設計、人聲生成、音效、音樂、氛圍語音及多音頻混合。核心採離散自迴歸生成器，直接在殘差向量量化（RVQ）token 上建模，脫離擴散 Transformer 連續生成範式。StepAudio Tokenizer 以 12.5 Hz 在共享 16×2048 殘差碼空間表示泛音頻，聯同量化語義與波形級聲學特徵。主幹模型沿時間軸自迴歸預測第一碼本，輕量級因果 Transformer 沿碼本軸補全其餘十五碼本。提出三大設計原則：干擾感知漸進式預訓練、RVQ Adapter、共享表示上的離散自迴歸建模。在 TTS 與聲音設計達 SOTA，同時保持語音、人聲、音效、音樂的強生成能力。

## 核心價值

首個在單一離散自迴歸框架統一語音與泛音頻生成的模型，證明 RVQ token 共享空間可同時保留語義與聲學資訊，為泛音頻生成確立新範式。

## 應用情境與實務影響

單一模型支援 TTS、語音編輯、歌聲合成、音效/音樂生成、語音翻譯等多樣任務，簡化部署管線；開源樣本頁面提供參考實作。

## 補充細節

論文於 2026-09-11 提交 (v1)，2026-09-14 發布。作者團隊超過 60 人（StepAudio LLM 團隊）。音頻樣本：stepaudiollm.github.io/step-audio-3-gen/。主體：Sound (cs.SD)、Audio and Speech Processing (eess.AS)。

## 維護紀錄

- 收錄日期：2026-09-17
- 最後更新：2026-09-17

---
title: "Microsoft 發布 MAI-Voice-1 與 MAI-Transcribe-1：自研語音模型登陸 Foundry，WER 達行業最低"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-04-02"
organization: "Microsoft"
source_url: "https://microsoft.ai/news/today-were-announcing-3-new-world-class-mai-models-available-in-foundry"
date_collected: "2026-07-29"
date_updated: "2026-07-29"
tags:
  - ai
  - tool
---

# Microsoft 發布 MAI-Voice-1 與 MAI-Transcribe-1：自研語音模型登陸 Foundry，WER 達行業最低

## 基本資訊

- 發布日期：2026-04-02
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://microsoft.ai/news/today-were-announcing-3-new-world-class-mai-models-available-in-foundry

## 概要

Microsoft AI 團隊於 2026 年 4 月 2 日（6 月 9 日更新）正式發布三款自研 MAI 模型並上線 Microsoft Foundry：MAI-Transcribe-1（語音轉文字）、MAI-Voice-1（文字轉語音）與 MAI-Image-2。MAI-Transcribe-1 在 FLEURS 25 語言基準上達到整體最低平均 WER（3.8%），在 11 種核心語言排名第一，其餘 14 語言均優於 Whisper-large-v3；MAI-Voice-1 單 GPU 1 秒內生成 60 秒語音，支援秒級語音克隆與長內容說話人身份保持，定價 $22/百萬字元。

## 核心價值

微軟首次以自研超大規模語音模型（MAI 系列）直接對標 OpenAI Whisper、ElevenLabs 等廠商，並在自家產品（Copilot 語音模式、Audio Expressions、Podcast 功能）大規模驗證後開放給 Foundry 開發者。

## 應用情境與實務影響

開發者可透過 Azure Speech、LLM Speech API 或 Foundry Model Catalog 直接調用；MAI-Transcribe-1 批次轉錄速度比 Azure Fast 快 2.5 倍、價格 $0.36/小時；MAI-Voice-1 支援 70+ 語言、自訂聲音建立，適用於即時對話代理、有聲書生產、無障碍工具等場景。

## 補充細節

MAI-Transcribe-1 針對 25 大語言優化，抗口噪、背景音與方言能力強；企業級 SLA 支援。MAI-Voice-1 採用流式架構，首音節延遲極低，適合 Realtime API 整合。兩模型皆由 Microsoft AI Superintelligence 團隊內部從頭訓練，非開源模型微調。定價具競爭力：轉錄 $0.36/小時、語音合成 $22/百萬字元。已整合至 Copilot Voice Mode、Dictation、Audio Expressions 等第一方產品驗證穩定性。

## 維護紀錄

- 收錄日期：2026-07-29
- 最後更新：2026-07-29

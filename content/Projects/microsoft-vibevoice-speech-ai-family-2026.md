---
title: "Microsoft VibeVoice: Open-Source Frontier Voice AI Family (ASR + TTS)"
type: project
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-03-06"
organization: "Microsoft"
source_url: "https://microsoft.github.io/VibeVoice"
date_collected: "2026-08-12"
date_updated: "2026-08-12"
tags:
  - ai
  - project
---

# Microsoft VibeVoice: Open-Source Frontier Voice AI Family (ASR + TTS)

## 基本資訊

- 發布日期：2026-03-06
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://microsoft.github.io/VibeVoice

## 概要

Microsoft 開源 VibeVoice 語音 AI 模型家族，包含 VibeVoice-TTS（長篇多講者語音合成，單次最長 90 分鐘、支援 4 位講者自然輪流）與 VibeVoice-ASR（統一語音轉文字，單次處理 60 分鐘長音訊，輸出講者、時間戳與內容，支援 50+ 語言與代碼切換）。VibeVoice-TTS 以 ICLR 2026 Oral 入選；VibeVoice-ASR 於 2026-03-06 整合進 Hugging Face Transformers 庫，2026-03-12 上線 Azure AI Foundry Labs。全系列採 MIT 許可證。

## 核心價值

提供業界領先的開源長篇多講者 TTS 與長音訊 ASR 基座，統一解決講者一致性、自然輪流、多語言識別等難題，大幅降低語音 AI 應用門檻。

## 應用情境與實務影響

開發者可直接透過 Transformers、Azure 或 GitHub 部署生產級語音識別與合成，應用於播客生成、會議記錄、多語言客服、即時翻譯等場景。

## 補充細節

VibeVoice-TTS：基於下一個 token 擴散與高效連續語音分詞器，ICLR 2026 Oral，2025-08-25 開源。VibeVoice-ASR：Whisper 風格編碼器-解碼器，內建講者分離，2026-01-21 開源。專案頁面：https://microsoft.github.io/VibeVoice/。Simon Willison 技術評測：https://simonwillison.net/2026/Apr/27/vibevoice/

## 維護紀錄

- 收錄日期：2026-08-12
- 最後更新：2026-08-12

---
title: "OpenAI 發布 GPT-Live-Transcribe 與 GPT-Transcribe：新一代語音轉文字模型"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-07-28"
organization: "OpenAI"
source_url: "https://community.openai.com/t/gpt-live-transcribe-and-gpt-transcribe-two-new-transcription-models-in-the-api/1388318"
date_collected: "2026-09-20"
date_updated: "2026-09-20"
tags:
  - ai
  - tool
---

# OpenAI 發布 GPT-Live-Transcribe 與 GPT-Transcribe：新一代語音轉文字模型

## 基本資訊

- 發布日期：2026-07-28
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://community.openai.com/t/gpt-live-transcribe-and-gpt-transcribe-two-new-transcription-models-in-the-api/1388318

## 概要

OpenAI 於 2026 年 7 月 28 日正式推出兩款新語音轉文字模型：GPT-Live-Transcribe（低延遲即時轉錄）與 GPT-Transcribe（非同步批次轉錄優化）。兩模型均支援上下文感知 ASR，可接受自由文本上下文、關鍵字提示、預期語言與歷史轉錄輪次作為輔助。在 22 語言 Common Voice 測試中，GPT-Transcribe 達 19.27% 字錯率，大幅優於 Whisper-1 的 40.37%。GPT-Live-Transcribe 定價 $0.017/分鐘（約 $1/小時）。

## 核心價值

取代 Whisper 成為 OpenAI 官方推薦轉錄模型，引入上下文感知機制顯著提升專有名詞、數字、口語與嘈雜環境下的準確度，並提供即時與批次兩條部署路徑。

## 應用情境與實務影響

開發者可直接遷移現有 Whisper 整合，獲得更高準確度與上下文注入能力；即時模型支援語音助手、會議紀錄、客服機器人等低延遲場景。

## 補充細節

模型支援關鍵字提示、多語言提示、語言偵測回報。API 端點相容現有 /v1/audio/transcriptions，遷移指南已發布於 OpenAI Cookbook。同期另發布 GPT-Live 語音生成模型（7/8）並於 7/31 加入 SynthID 水印驗證。

## 維護紀錄

- 收錄日期：2026-09-20
- 最後更新：2026-09-20

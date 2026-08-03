---
title: "Mistral 發布 Voxtral TTS：4B 參數多語言零樣本語音合成模型"
type: technical-development
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-03-26"
organization: "Mistral AI"
source_url: "https://mistral.ai/news/voxtral-tts"
date_collected: "2026-08-04"
date_updated: "2026-08-04"
tags:
  - ai
  - technical-development
---

# Mistral 發布 Voxtral TTS：4B 參數多語言零樣本語音合成模型

## 基本資訊

- 發布日期：2026-03-26
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://mistral.ai/news/voxtral-tts

## 概要

Mistral AI 於 2026 年 3 月 26 日發布 Voxtral TTS，為首個文字轉語音模型，4B 參數輕量化設計可於消費級硬體運行。支援 9 種語言，3 秒音訊即可零樣本語音克隆，捕捉口音、語調、語氣詞等細微特徵。人類偏好測試超越 ElevenLabs Flash v2.5，延遲極低（典型輸入 70ms 首音延遲，RTF ≈9.7x），原生支援最長 2 分鐘連續生成。採 Apache 2.0 開放權重授權。

## 核心價值

歐洲實驗室以開放權重挑戰商業 TTS 龍頭，兼顧品質、延遲與部署成本，推動語音代理大規模落地。

## 應用情境與實務影響

企業可自建語音客服、有聲書、無障礙服務，無供應商鎖定；低延遲適合即時雙向語音代理；API 定價 $0.016/千字符極具成本優勢。

## 補充細節

架構基於 Ministral 3B 的 transformer 自回歸 flow-matching 模型。可與 Voxtral Transcribe 組合成端到端語音對話，或接入任意 STT+LLM 棧。Mistral Studio 提供試用介面。同期另發布 Voxtral Small/Mini 語音轉文字模型（2025/07 發布，2026/02 更新 Realtime 版本）。

## 維護紀錄

- 收錄日期：2026-08-04
- 最後更新：2026-08-04

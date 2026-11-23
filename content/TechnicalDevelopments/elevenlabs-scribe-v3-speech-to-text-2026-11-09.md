---
title: "ElevenLabs 發布 Scribe v3 / v3 Live：最精準語音辨識模型支援 102 語言"
type: technical-development
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-11-09"
organization: "ElevenLabs"
source_url: "https://elevenlabs.io/blog/scribe-v3"
date_collected: "2026-11-24"
date_updated: "2026-11-24"
tags:
  - ai
  - technical-development
---

# ElevenLabs 發布 Scribe v3 / v3 Live：最精準語音辨識模型支援 102 語言

## 基本資訊

- 發布日期：2026-11-09
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://elevenlabs.io/blog/scribe-v3

## 概要

ElevenLabs 於 2026 年 11 月 9 日正式推出 Scribe v3（批次轉錄）與 Scribe v3 Live（即時轉錄），為其語音辨識產品線最新旗艦。Scribe v3 在 FLEURS 102 語言基準上字錯率較 v2 降低 27%，並超越 GPT-Transcribe、Deepgram Nova-3、Gemini 3.5 Transcribe 等競品；Scribe v3 Live 語義字錯率較 v2 Realtime 降 44%，中位延遲 150 ms。新增數字格式化、混合語言支援、關鍵詞庫（至 1 萬詞）、發言人偵測（最多 32 位）、輪替預測提交策略。API 僅需將 model_id 改為 scribe_v3 / scribe_v3_live 即可無縫遷移。

## 核心價值

單一模型同時達成 SOTA 多語言批次準確度與超低延遲即時轉錄，並內建發言人標記、關鍵詞強制修正、混語處理等生產級功能，大幅降低語音代理與會議紀錄應用的整合門檻。

## 應用情境與實務影響

語音代理、客服機器人、會議記錄、內容創作者字幕生成等場景可直接升級準確度與延遲；關鍵詞庫解決專有名詞辨識痛點；輪替預測改善即時轉錄斷句自然度；向下相容 v2 遷移零成本。

## 補充細節

同日文檔更新日誌 (elevenlabs.io/docs/changelog/2026/11/9) 同步釋出。Scribe v2 / v2 Realtime 維持可用。模型透過 ElevenAPI、ElevenAgents、雲端 App 皆可呼叫。企業級可申請內部部署。公司近期完成 1.8 億美元融資，估值 33 億美元。

## 維護紀錄

- 收錄日期：2026-11-24
- 最後更新：2026-11-24

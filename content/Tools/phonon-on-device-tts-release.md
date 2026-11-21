---
title: "Phonon：Gradium 開源終端裝置 TTS 模型家族"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-10-20"
organization: "Gradium"
source_url: "https://gradium.ai/blog/release-phonon-open-weight"
date_collected: "2026-11-22"
date_updated: "2026-11-22"
tags:
  - ai
  - tool
---

# Phonon：Gradium 開源終端裝置 TTS 模型家族

## 基本資訊

- 發布日期：2026-10-20
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://gradium.ai/blog/release-phonon-open-weight

## 概要

Kyutai 實驗室衍生創企 Gradium 於 2026 年 10 月 20 日發布 Phonon，首個面向終端裝置的開源權重 TTS 模型家族。包含 31M 參數英文模型（Apache 2.0，64 MB）與 40M 參數多語言模型（CC BY-NC 4.0，支援英法德西葡五語言語音克隆）。架構繼承 Pocket TTS 與 Mimi 編解碼器，因果 Transformer + 一步流匹配頭，12.5 Hz 連續音頻潛變量生成，可串流、首包 30–100 ms（CPU）、WER 1.00%（Seed-TTS 英文基準）。提供 Rust 推理運行時、Hugging Face Transformers 整合、瀏覽器 WebGPU Demo。

## 核心價值

將 SOTA 級 TTS 壓縮至 31M/40M 參數並開源權重，證明終端裝置即時語音合成已具備生產級品質，消除雲端延遲與隱私疑慮。

## 應用情境與實務影響

手機、筆電、單板機、瀏覽器即可離線即時合成語音；適用 NPC 語音、離線助理、隱私敏感場合；Rust 運行時便於嵌入式整合；Hugging Face 整合降低採用門檻。

## 補充細節

官方部落格 gradium.ai 於 2026-10-20 發布《Open-Sourcing Phonon: A Suite of Frontier On-Device TTS Models》，同步於 NVIDIA GTC Berlin 現場演示。31M 模型在 MacBook Pro M2 單核 CPU 30–100 ms 首音；40M 多語言模型跨五語言聲音克隆；在法德西三語言 WER 比 NVIDIA Magpie 低 3.5 倍、參數少 3.6 倍。Hugging Face Transformers 於 2026-10-20 納入文檔（gradium_phonon_tts）。模型卡：gradium/phonon-31m-en、gradium/phonon-40m-multilingual。

## 維護紀錄

- 收錄日期：2026-11-22
- 最後更新：2026-11-22

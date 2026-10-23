---
title: "PhonoVoxtLM：單一碼本音韻標記統一語音理解與生成"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-10-22"
organization: "作者單位未在摘要中明示（arXiv:2610.18469v1）"
source_url: "https://arxiv.org/html/2610.18469v1"
date_collected: "2026-10-24"
date_updated: "2026-10-24"
tags:
  - ai
  - paper
---

# PhonoVoxtLM：單一碼本音韻標記統一語音理解與生成

## 基本資訊

- 發布日期：2026-10-22
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/html/2610.18469v1

## 概要

論文提出 PhonoVoxtLM，基於 VoxtLM 框架，採用單一碼本音韻標記（phonological tokens）同時支援語音理解（ASR、語音辨識）與生成（TTS）。該標記器聯合訓練 ASR 與語音重合成目標，以可微 k-means 保留語言內容與韻律資訊。實驗顯示在平衡資料設定下，ASR WER 從 7.1%/17.8% 降至 4.2%/8.6%，F0 相關係數從 0.167 升至 0.282，全面優於 HuBERT 基線。

## 核心價值

證明單一碼本音韻標記可作為理解與生成的共享表示，無需額外語音標記預測模組，簡化架構並提升雙向效能。

## 應用情境與實務影響

為統一語音語言模型提供更簡潔的標記化方案；降低多任務語音模型部署複雜度；音韻標記器權重公開可直接複用。

## 補充細節

使用預訓練 Phonological Tokenizer (Onda et al., 2026)，WavLM-large encoder 第 21 層特徵 + K=2000 碼本；encoder 與碼本凍結；在 VoxtLM 架構上適配；評估涵蓋語音辨識、辨別、TTS 多項指標。

## 維護紀錄

- 收錄日期：2026-10-24
- 最後更新：2026-10-24

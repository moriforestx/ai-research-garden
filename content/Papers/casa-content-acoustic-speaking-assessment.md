---
title: "CASA: Content-Acoustic Speaking Assessment with Speech Encoder and Large Language Model"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-08-13"
organization: "Nhan Phan, Ilona Lähteenmäki, Anna von Zansen, Olli-Pekka Pauna, Yaroslav Getman, Tamás Grósz, Mikko Kurimo"
source_url: "https://arxiv.org/abs/2608.13101"
date_collected: "2026-08-17"
date_updated: "2026-08-17"
tags:
  - ai
  - paper
---

# CASA: Content-Acoustic Speaking Assessment with Speech Encoder and Large Language Model

## 基本資訊

- 發布日期：2026-08-13
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2608.13101

## 概要

提出 CASA，結合 Whisper-medium 語音編碼器與 Qwen3.5-2B 大語言模型的自動口語評估架構，在 Speak & Improve Corpus 2025 達到 RMSE 0.358 的 SOTA 表現，推論參數量僅為前人一半。架構將聲學（流暢度、發音）與內容（語法、詞彙、連貫性）資訊解耦，提供更可解釋的評估；僅需三個手工流暢度特徵即可泛化至其他 ASA 語料庫。透過消融實驗與重複運行，分析聲學與內容資訊的個別與互補貢獻，並展示 LLM 推理在無訓練內容驗證的潛力。

## 核心價值

證明輕量級語音編碼器 + LLM 的簡潔架構即可達到 SOTA，並提供聲學/內容可解釋的分離評估。

## 應用情境與實務影響

為語言學習應用、自動口語考試評分提供低參數量、高可解釋性的解決方案；架構可無縫遷移至其他口語評估語料。

## 補充細節

代碼：https://github.com/aalto-speech/casa；將提交 ICASSP 2027。發布日期以 arXiv citation_date (2026-08-13) 為準。

## 維護紀錄

- 收錄日期：2026-08-17
- 最後更新：2026-08-17

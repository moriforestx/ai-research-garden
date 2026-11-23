---
title: "Google DeepMind 發布 EmbeddingGemma 2：原生多模態嵌入模型"
type: technical-development
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-06"
organization: "Google DeepMind"
source_url: "https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2"
date_collected: "2026-11-24"
date_updated: "2026-11-24"
tags:
  - ai
  - technical-development
---

# Google DeepMind 發布 EmbeddingGemma 2：原生多模態嵌入模型

## 基本資訊

- 發布日期：2026-10-06
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2

## 概要

Google DeepMind 於 2026 年 10 月 6 日正式發布 EmbeddingGemma 2，一個 7.4 億參數的開源多模態嵌入模型，原生支援文字、程式碼、圖像、影片與音訊四大模態在單一 768 維向量空間中的統一表示。模型採分階段課程訓練、簡化逐層嵌入與模組化編碼器設計，在 MIEB 等綜合基準上建立新 Pareto 前緣，超越專用模型與 2-12 倍參數量的競品。釋出 Apache 2.0 授權權重、Hugging Face 模型卡、量化權重與截斷嵌入支援，適合裝置端推論。

## 核心價值

首個原生四模態統一嵌入的開源輕量模型，單一模型即可跨模態檢索（如以語音查找影片片段），並支援矩陣式資源權衡（選擇性載入編碼器、可調視覺 token 預算、可截斷嵌入維度、量化權重）。

## 應用情境與實務影響

大幅降低多模態 RAG 與裝置端語義搜尋的部署門檻；與 Gemma 4 共享 tokenizer 與音訊編碼器，聯合管線記憶體占用更低；開源授權促進社群二次開發與學術研究。

## 補充細節

arXiv 預印本 (2610.37364) 於 10/27 提交 v1、11/9 更新 v2。DeepMind 官方出版物頁面同步於 10/27 上線。模型總參數 7.4 億，含 2.7 億文字、1.7 億視覺、3 億音訊編碼器。Hugging Face 首月下載超 60 萬次。

## 維護紀錄

- 收錄日期：2026-11-24
- 最後更新：2026-11-24

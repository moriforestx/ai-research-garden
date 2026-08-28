---
title: "NVIDIA Nemotron 3.5 ASR Streaming 語音識別模型"
type: technical-development
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-04"
organization: "NVIDIA"
source_url: "https://huggingface.co/nvidia/nemotron-3.5-asr-streaming-0.6b"
date_collected: "2026-08-29"
date_updated: "2026-08-29"
tags:
  - ai
  - technical-development
---

# NVIDIA Nemotron 3.5 ASR Streaming 語音識別模型

## 基本資訊

- 發布日期：2026-06-04
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://huggingface.co/nvidia/nemotron-3.5-asr-streaming-0.6b

## 概要

NVIDIA 於 2026 年 6 月 4 日發布 Nemotron 3.5 ASR Streaming 模型，這是一個 600M 參數的 cache-aware 流式自動語音識別(ASR)模型，支援 40 語言-地區組合（約 36 種語言）在單一 checkpoint 中。提供 runtime-configurable 的 chunk sizes (80ms-1120ms)，原生支援標點符號和大小寫，且相比傳統 buffered 方法具有 3x 更高的 GPU 併發度。

## 核心價值

流式設計與多語言支援，實現低延遲高吞吐量的語音識別

## 應用情境與實務影響

適用於需要即時語音轉文字的應用，如語音助手、會議紀錄、客服系統和多語言即時翻譯

## 補充細節

採用 Cache-Aware FastConformer-RNNT 架構，避免重複計算，僅處理新音訊區塊同時重用編碼器上下文。在 80ms 延遲設定下可支援約 17× 更多併發串流。模型在多樣聲學條件下進行訓練，提供語言 ID 提示條件選項和自動語言偵測。已在 Hugging Face Transformers (AutoModelForRNNT) 和 NVIDIA NeMo 框架中提供。

## 維護紀錄

- 收錄日期：2026-08-29
- 最後更新：2026-08-29

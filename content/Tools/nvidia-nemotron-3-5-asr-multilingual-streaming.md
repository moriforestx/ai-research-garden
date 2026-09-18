---
title: "NVIDIA Nemotron 3.5 ASR: Multilingual Streaming Speech Recognition"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-11"
organization: "NVIDIA"
source_url: "https://build.nvidia.com/nvidia/nemotron-asr-streaming/modelcard"
date_collected: "2026-09-19"
date_updated: "2026-09-19"
tags:
  - ai
  - tool
---

# NVIDIA Nemotron 3.5 ASR: Multilingual Streaming Speech Recognition

## 基本資訊

- 發布日期：2026-06-11
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://build.nvidia.com/nvidia/nemotron-asr-streaming/modelcard

## 概要

NVIDIA 發布 Nemotron 3.5 ASR，一個 6 億參數的多語言流式自動語音辨識模型，支援 40 種語言與地區，具備自動語言偵測功能。採用 Cache-Aware FastConformer-RNNT 架構，透過快取編碼器上下文消除冗餘重疊計算，實現零重疊的低延遲流式推理，原生輸出標點與大小寫。模型以開放權重形式透過 NVIDIA NGC、Hugging Face 與 NIM 容器發布，採 OpenMDW-1.1 授權，可商用。

## 核心價值

首個單一模型支援 40 語言、具備自動語言偵測與快取感知流式架構的開放權重 ASR，大幅降低多語言部署複雜度與推理延遲。

## 應用情境與實務影響

可直接部署於即時語音助理、客服轉錄、多語言會議字幕等生產環境；單一模型替代多個語言專用模型，簡化維運；H100 上可維持極高併發流數，降低單位成本。

## 補充細節

600M 參數，FastConformer-RNNT (24-layer encoder + RNNT decoder)，支援 80/160/320/560/1120ms chunk size，OpenMDW-1.1 授權，Hugging Face: nvidia/nemotron-3.5-asr-streaming-0.6b，NGC 容器可用。

## 維護紀錄

- 收錄日期：2026-09-19
- 最後更新：2026-09-19

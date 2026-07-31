---
title: "TurboVLA：即時視覺語言動作模型，在 RTX 4090 上以 32 Hz、<1 GB VRAM 執行"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-29"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2607.27205"
date_collected: "2026-08-01"
date_updated: "2026-08-01"
tags:
  - ai
  - paper
---

# TurboVLA：即時視覺語言動作模型，在 RTX 4090 上以 32 Hz、<1 GB VRAM 執行

## 基本資訊

- 發布日期：2026-07-29
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2607.27205

## 概要

TurboVLA 提出新型視覺語言動作 (VLA) 範式，移除傳統 LLM 為中心的 V→L→A 架構，改為直接 V+L→A 映射。使用 DINOv3 編碼視覺、BERT 編碼語言，經輕量雙向交叉注意力交換資訊，再由精簡解碼器預測動作區塊。模型僅 0.2B 參數，在 RTX 4090 上達 32 Hz 推理頻率、<1 GB VRAM、31 ms 延遲，於多項機器人任務達 98% 成功率。代碼開源。

## 核心價值

證明無需大型 LLM 即可達成即時機器人控制，重新定義 VLA 架構為輕量視覺語言直接互動，大幅降低部署門檻至消費級 GPU。

## 應用情境與實務影響

機器人研究者可在單張 RTX 4090 上訓練與部署高頻 VLA 政策；邊緣機器人、桌面級實驗平台不再需要多張 A100/H100。開源代碼可直接整合現有資料管線。

## 補充細節

arXiv:2607.27205v1，提交於 2026-07-29。類別：cs.CV、cs.RO。作者提供代碼連結。架構創新在於移除 LLM 核心，改用 DINOv3 視覺骨幹 + BERT 文本編碼器 + 輕量交叉注意力 + 動作區塊解碼器，參數量僅 0.2B。實驗涵蓋模擬與真實機器人任務，展現零樣本泛化能力。

## 維護紀錄

- 收錄日期：2026-08-01
- 最後更新：2026-08-01

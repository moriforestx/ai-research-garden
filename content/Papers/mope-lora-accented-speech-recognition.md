---
title: "MoPE-LoRA：基於音素專家混合的低秩適配，用於口音英語語音識別"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-10-13"
organization: "多機構合作"
source_url: "https://arxiv.org/abs/2610.26888"
date_collected: "2026-10-23"
date_updated: "2026-10-23"
tags:
  - ai
  - paper
---

# MoPE-LoRA：基於音素專家混合的低秩適配，用於口音英語語音識別

## 基本資訊

- 發布日期：2026-10-13
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2610.26888

## 概要

論文提出 Mixture of Phonetic Experts based Low-Rank Adaptation (MoPE-LoRA)，一種針對口音英語語音識別的參數高效適配框架。與以往按口音分配專家的方法不同，MoPE-LoRA 依發音方式類別劃分六個固定低秩專家，並在幀級透過音素監督與聲學門控的混合機制進行路由。專家組跨口音共享，無需口音專用模組，自然支援未見過的口音。在 L2-ARCTIC 基準上，MoPE-LoRA 持續優於單一 LoRA 與全量微調；零樣本評估（訓練時保留一口音）中，相對單一 LoRA 取得 12.3% 相對改進。

## 核心價值

將適配軸心從口音層級轉向音素層級，實現跨口音泛化且無需增加口音專用參數；獲 Interspeech 2026 接收。

## 應用情境與實務影響

多口音 ASR 部署可大幅減少適配參數量與維護成本；對低資源口音、零樣本泛化場景具高實用價值。

## 補充細節

Interspeech 2026 (Sydney) 接收論文；5 頁、3 圖、6 表；DOI: 10.21437/Interspeech.2026-322。作者來自多機構合作。

## 維護紀錄

- 收錄日期：2026-10-23
- 最後更新：2026-10-23

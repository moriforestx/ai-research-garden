---
title: "V-RAE: Rethinking Video Latent Spaces for Generation"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-08-13"
organization: "Minghui Guo, Shengqiong Wu, Hao Fei"
source_url: "https://arxiv.org/abs/2608.13556"
date_collected: "2026-08-17"
date_updated: "2026-08-17"
tags:
  - ai
  - paper
---

# V-RAE: Rethinking Video Latent Spaces for Generation

## 基本資訊

- 發布日期：2026-08-13
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2608.13556

## 概要

提出 V-RAE（Video Representation Autoencoder），一種針對生成任務優化的視頻潛在空間自編碼器。傳統視頻自編碼器主要優化像素級重建，但重建最優的潛在空間不一定適合生成建模。V-RAE 在凍結的視覺基礎模型表示之上構建緊湊生成潛在向量，輕量級時間池化模組移除時間冗餘同時保留語義結構，視頻解碼器從壓縮特徵重建連續運動。在 K600 上達到 2.13 rFVD，優於所有評測的大規模預訓練視頻 VAE；其潛在向量保留顯著更多語義資訊。生成設定下在 UCF101 (gFVD 117.86) 和 K600 (gFVD 19.16) 達到 SOTA，收斂速度快達 6 倍。引入 tFVD 作為時間連貫性診斷，比重建質量更能預測下游生成品質。亦在 Cityscapes 未來視頻預測優於 Wan 2.2 VAE 潛在空間。

## 核心價值

證明凍結語義表示可同時支援視頻重建、生成與預測建模；重建質量不足以表徵生成效用，需引入時間連貫性指標。

## 應用情境與實務影響

為視頻生成提供更高效、語義更豐富的潛在空間，大幅加速收斂並提升生成品質，可直接應用於視頻生成、預測等下游任務。

## 補充細節

專案頁面：https://v-rae.github.io/；arXiv:2608.13556，26 頁、8 表、13 圖。使用四種代表性凍結編碼器評測。發布日期以 arXiv citation_date (2026-08-13) 為準。

## 維護紀錄

- 收錄日期：2026-08-17
- 最後更新：2026-08-17

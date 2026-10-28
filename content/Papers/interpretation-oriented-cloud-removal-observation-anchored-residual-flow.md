---
title: "Interpretation-Oriented Cloud Removal via Observation-Anchored Residual Flow with Geo-Contextual Alignment"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-02"
organization: "The Chinese University of Hong Kong, Shenzhen; Shanghai AI Lab"
source_url: "https://arxiv.org/abs/2607.02471v1"
date_collected: "2026-10-29"
date_updated: "2026-10-29"
tags:
  - ai
  - paper
---

# Interpretation-Oriented Cloud Removal via Observation-Anchored Residual Flow with Geo-Contextual Alignment

## 基本資訊

- 發布日期：2026-07-02
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2607.02471v1

## 概要

CUHK-Shenzhen 與 Shanghai AI Lab 團隊提出 Geo-Anchored Cloud Removal (GACR) 框架，針對光學遙感雲移除任務，同時兼顧重建保真度與下游解讀任務（語意分割、變化偵測、建築物偵測等）準確率。核心創新為：(1) Observation-Anchored Residual Flow (OAR-Flow) —— 將雲移除重構為以觀測雲圖為錨點的殘差反演過程，而非從純雜訊生成，實現快速、穩定、高保真重建；(2) Geo-Contextual Prior Alignment (GCPA) —— 引入視覺基礎模型 (VFM) 語義流形約束重建軌徑，嚴格保持複雜地景的空間語義完整性。跨六大雲移除資料集與十二項下游任務驗證，GACR 重建品質領先 SOTA，且一致提升下游任務準確率。代碼開源於 GitHub。

## 核心價值

首創「觀測錨點殘差流」與「地理語境語義對齊」雙重機制，解決傳統雲移除重視視覺真實感而忽略下游語義保真度的長期痛點，為遙感解讀鏈路提供端到端品質保證。

## 應用情境與實務影響

直接服務衛星影像預處理管線，顯著提升語意分割、建築物偵測、高程估測等下游任務可靠度；OAR-Flow 快速推理特性適合近即時遙感應用。VFM 語義約束範式可推廣至去霧、超分辨率等遙感復原任務。

## 補充細節

OAR-Flow 基於概率流 ODE，以雲圖為初始條件學習殘差速度場，理論證明收斂至無雲分布。GCPA 以 DINOv2/CLIP 等 VFM 提取語義先驗，透過特徵空間對齊損失正則化生成軌徑。於 CUHKCR-EXT、WHU-CD 等基準達最高 PSNR/SSIM；下游 U-Net、DeepLabv3+、Mask R-CNN 等架構均獲一致增益。接受 ECCV 2026。

## 維護紀錄

- 收錄日期：2026-10-29
- 最後更新：2026-10-29

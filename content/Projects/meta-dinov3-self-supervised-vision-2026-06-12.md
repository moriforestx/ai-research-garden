---
title: "Meta 發布 DINOv3：以 17 億圖像自監督預訓練的通用視覺基座模型"
type: project
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-12"
organization: "Meta AI Research (FAIR)"
source_url: "https://ai.meta.com/blog/dinov3-self-supervised-vision-model"
date_collected: "2026-11-11"
date_updated: "2026-11-11"
tags:
  - ai
  - project
---

# Meta 發布 DINOv3：以 17 億圖像自監督預訓練的通用視覺基座模型

## 基本資訊

- 發布日期：2026-06-12
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://ai.meta.com/blog/dinov3-self-supervised-vision-model

## 概要

Meta AI 於 2026 年 6 月 12 日正式發布 DINOv3，一系列自監督視覺 Transformer 骨幹網路，於 17 億張無標註圖像上預訓練，參數量從 21M 到 7B。單一凍結骨幹在物件偵測、語意分割等稠密預測任務上超越專用模型，並開放商業授權的模型權重、下游評測頭與範例筆記本。GitHub 同步釋出訓練代碼與衛星/醫學影像適配配方（FINO 分支）。

## 核心價值

證明大規模自監督預訓練可產出通用、免微調的視覺特徵，大幅降低標註資料依賴，並以開放權重加速下游應用落地。

## 應用情境與實務影響

提供即插即用的 SOTA 視覺骨幹，適用於分割、偵測、追蹤、衛星圖像分析、醫學影像等領域；Hugging Face 整合降低部署門檻。

## 補充細節

模型家族涵蓋 ViT-S/B/L/G/7B，含通用、衛星（MAXAR）、螢光顯微（HPA）三大預訓練域。釋出內容：PyTorch 參考實作、Hugging Face Transformers 整合、商業友善授權、下游評測頭、入門筆記本。CHMv2 樹冠高度圖模型展示實務遷移效能（R² 從 0.53 提升至 0.86）。

## 維護紀錄

- 收錄日期：2026-11-11
- 最後更新：2026-11-11

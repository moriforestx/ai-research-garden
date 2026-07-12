---
type: paper
title: "Advancing Vision Transformer with Enhanced Spatial Priors"
category: "Computer Vision"
score: "4"
date_collected: "2026-07-12"
published_date: "2026-04-18"
source_url: "https://arxiv.org/abs/2604.18549"
tags:
  - ai
  - paper
  - computer-vision
  - vision-transformer
---

# Advancing Vision Transformer with Enhanced Spatial Priors

## 基本資訊

- 類別：Computer Vision
- 日期：2026-04-18
- 新鮮度：0–3 個月
- Source：https://arxiv.org/abs/2604.18549
- Score：4

## 摘要

本文提出一種增強空間先驗的 Vision Transformer 改進方案。標準 ViT 缺乏固有的空間感知能力，導致在物體檢測、實例分割等密集預測任務上表現遜於 CNN 基礎模型。作者通過引入可學習的空間位置編碼和局部注意力機制，顯著提升 ViT 在下游密集預測任務的性能，在 COCO 物體檢測和 ADE20K 語義分割基準上達到新 SOTA。

## 核心重點

- 引入增強空間位置編碼，賦予 ViT 更強的空間感知能力
- 設計局部注意力機制，結合全局注意力與局部卷積優勢
- 在 ImageNet-1K 分類、COCO 檢測、ADE20K 分割三大基準全面超越同規模基線
- 提供即插即用模組，可無縫替換現有 ViT 骨幹

## 為什麼重要

Vision Transformer 作為視覺基礎模型主流架構，其缺乏空間先驗長期被詬病。本文從架構層面系統性解決此問題，不依賴龐大預訓練數據即可獲得顯著提升，極大降低了 ViT 在密集預測任務的應用門檻。

## 可能影響

- 推動 Vision Transformer 在自動駕駛感知、醫療影像分析、遙感影像解讀等密集預測場景的實際落地
- 為後續 ViT 改進工作提供標準化空間增強基線
- 可能成為下一代視覺基礎模型（如 SAM 2、DINOv3）的標配組件

## 相關概念

- [[Vision Transformer]]
- [[Object Detection]]
- [[Image Segmentation]]
- [[Spatial Position Encoding]]
- [[Dense Prediction]]

## 更新紀錄

- 2026-07-12：首次收錄。

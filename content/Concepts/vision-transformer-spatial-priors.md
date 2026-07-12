---
type: concept
name: "Vision Transformer Spatial Priors"
date_updated: "2026-07-12"
tags:
  - concept
  - computer-vision
  - vision-transformer
  - spatial-priors
---

# Vision Transformer Spatial Priors

## 定義

為 Vision Transformer 引入空間感知先驗知識的架構增強技術。標準 ViT 將圖像分塊序列化後完全依賴自注意力學習空間關係，缺乏卷積神經網絡固有的平移不變性和局部性偏好。空間先驗注入方式：絕對/相對位置編碼增強、局部注意力窗口、可變形注意力、卷積混合塊、空間先驗正則化損失。代表工作：DAT/DAT++、Swin Transformer、ConvNeXt-ViT、ViT-Adapter、本日收錄的 Enhanced Spatial Priors ViT (arXiv:2604.18549)。

## 為什麼重要

- 解決 ViT 在密集預測任務（檢測、分割、姿態估計）上長期遜於 CNN 的根本原因
- 使 ViT 成為真正通用的視覺骨幹，統一分類與密集預測架構
- 為基礎模型（SAM、DINOv2、MAE）提供更強的空間推理能力

## 出現在哪些內容

- [[Advancing Vision Transformer with Enhanced Spatial Priors]]
- [[Daily/2026-07-12]]

## 相關概念

- [[Vision Transformer]]
- [[Object Detection]]
- [[Image Segmentation]]
- [[Deformable Attention]]
- [[Swin Transformer]]
- [[Dense Prediction]]

## 更新紀錄

- 2026-07-12：首次建立。

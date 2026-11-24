---
title: "Beyond the Last Layer: Global Inter-Layer Aggregation for AI-Generated Image Detection"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-11-01"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.00017"
date_collected: "2026-11-25"
date_updated: "2026-11-25"
tags:
  - ai
  - paper
---

# Beyond the Last Layer: Global Inter-Layer Aggregation for AI-Generated Image Detection

## 基本資訊

- 發布日期：2026-11-01
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2611.00017

## 概要

此研究針對 AI 生成圖像偵測任務，指出現有方法普遍僅使用預訓練視覺編碼器最後一層的全域特徵，忽略了中間層豐富的階層資訊。提出 GILA（Global Inter-Layer Aggregation）框架：將不同網路深度的全域表示視為有序序列，透過層間交互模組讓各層利用其他深度的上下文更新表示，再以自適應聚合模組依輸入樣本學習層權重，最後進行真偽分類。實驗在三種預訓練骨幹網路上驗證，GILA 優於單純使用最後一層的基線，在十種已見生成器與三種未見生成器上皆有顯著提升。

## 核心價值

證明多層全域特徵聚合能顯著提升 AI 生成圖像偵測的泛化能力，無需微調骨幹網路，提供即插即用的偵測增強方案。

## 應用情境與實務影響

為深度偽造偵測、內容真實性驗證、生成式 AI 治理提供更強健的技術基礎；模組化設計易於整合至現有偵測管線。

## 補充細節

方法：GILA 包含三階段——多層全域特徵提取、跨層情境化交互、樣本自適應聚合。使用凍結的預訓練編碼器（ViT-B/16、Swin-T、ConvNeXt-B），保留各編碼階段的 CLS token 或全域平均池化特徵。層間交互採用注意力機制，自適應聚合學習每層對當前樣本的重要性權重。資料集：GenImage、DRCT、DiffusionDB 等十種生成器；未見生成器包括 Midjourney v6、DALL-E 3、Stable Diffusion XL。結果：GILA 平均 AUC 提升 2.1-4.7%，在未見生成器上提升 5.3-8.9%。參數量僅增加 <1%。

## 維護紀錄

- 收錄日期：2026-11-25
- 最後更新：2026-11-25

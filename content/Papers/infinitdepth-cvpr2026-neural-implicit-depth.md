---
title: "InfiniDepth: Arbitrary-Resolution and Fine-Grained Depth Estimation with Neural Implicit Fields"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-20"
organization: "Computer Vision Foundation"
source_url: "https://openaccess.thecvf.com/content/CVPR2026/papers/Yu_InfiniDepth_Arbitrary-Resolution_and_Fine-Grained_Depth_Estimation_with_Neural_Implicit_Fields_CVPR_2026_paper.pdf"
date_collected: "2026-09-24"
date_updated: "2026-09-24"
tags:
  - ai
  - paper
---

# InfiniDepth: Arbitrary-Resolution and Fine-Grained Depth Estimation with Neural Implicit Fields

## 基本資訊

- 發布日期：2026-06-20
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026/papers/Yu_InfiniDepth_Arbitrary-Resolution_and_Fine-Grained_Depth_Estimation_with_Neural_Implicit_Fields_CVPR_2026_paper.pdf

## 概要

CVPR 2026 論文提出 InfiniDepth，利用神經隱式域建立深度表示，實現任意解析度與細膩粒度的單眼深度估計。透過視覺Transformer編碼輸入圖像、重組塊構建特徵金字塔，並在任意2D座標上進行局部窗口特徵聚合與深度查詢，突破固定解析度限制。

## 核心價值

首次將神經隱式域應用於單眼深度估計，支援任意解析度推理，同時保留細節與幾何一致性，為高解析度3D感知開啟新範式。

## 應用情境與實務影響

適用於自動駕駛、機器人導航、擴增實境等需高精度深度的場景；支援跨解析度遷移與細節保留的新視角合成。

## 補充細節

論文於 2026-02 被 CVPR 2026 接收，3 月發布推理碼。方法包括：(1) 視覺Transformer編碼器提取多階段特徵；(2) 重組塊建構特徵金字塔；(3) 對任意連續2D座標採樣局部窗口特徵，經輕量MLP預測深度；(4) 高斯頭提升新視角合成品質。在自建 Synth4K 4K基準上，較 SOTA 方法在深度誤差（AbsRel）降低 18.3%，細節保留度提升 22.7%。

## 維護紀錄

- 收錄日期：2026-09-24
- 最後更新：2026-09-24

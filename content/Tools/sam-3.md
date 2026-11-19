---
title: "Segment Anything Model 3 (SAM 3)：統一的概念提示檢測、分割與追蹤模型"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-11-19"
organization: "Meta AI (FAIR)"
source_url: "https://ai.meta.com/blog/segment-anything-model-3"
date_collected: "2026-11-20"
date_updated: "2026-11-20"
tags:
  - ai
  - tool
---

# Segment Anything Model 3 (SAM 3)：統一的概念提示檢測、分割與追蹤模型

## 基本資訊

- 發布日期：2026-11-19
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://ai.meta.com/blog/segment-anything-model-3

## 概要

Meta AI 於 2026 年 11 月 19 日正式發布 Segment Anything Model 3 (SAM 3)，統一了圖像與視頻中的檢測、分割與追蹤任務。支援文字提示、範例圖像與視覺提示三種概念提示方式，實現 Promptable Concept Segmentation (PCS)。模型包含圖像級檢測器與基於記憶的視頻追蹤器，共享單一骨幹網絡，透過存在性頭部解耦識別與定位。在 PCS 基準上較現有系統提升 2 倍，並開源模型權重、SA-Co 評測數據集與微調代碼。

## 核心價值

首個支援自然語言概念提示的統一視覺基礎模型，實現跨圖像/視頻的零樣本檢測、分割與身份一致的追蹤。

## 應用情境與實務影響

研究人員與開發者可透過 Segment Anything Playground 直接體驗，適用於野生動物監測、洪水應急響應、醫療影像分析等零樣本視覺任務，標註效率較人工提升 5 倍（負樣本）與 36%（正樣本）。

## 補充細節

同步發布 SAM 3D（3D 重建與人體姿態估計）、SAM Audio（音訊分離）與 Perception Encoder Audiovisual。SA-Co 數據集包含 400 萬唯一概念標籤。論文發表於 arXiv，代碼與權重開源授權。

## 維護紀錄

- 收錄日期：2026-11-20
- 最後更新：2026-11-20

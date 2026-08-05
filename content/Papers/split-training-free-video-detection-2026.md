---
title: "SPLIT: Training-Free AI-Generated and Partially Edited Video Detection via Spatial Patch-Level Incoherence and Temporal Roughness"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-03"
organization: "ECCV 2026"
source_url: "https://arxiv.org/abs/2607.02886"
date_collected: "2026-08-06"
date_updated: "2026-08-06"
tags:
  - ai
  - paper
---

# SPLIT: Training-Free AI-Generated and Partially Edited Video Detection via Spatial Patch-Level Incoherence and Temporal Roughness

## 基本資訊

- 發布日期：2026-07-03
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2607.02886

## 概要

提出 SPLIT，一個無需訓練即可偵測 AI 生成與部分編輯影片的方法。利用凍結視覺編碼器的 patch token，結合兩階段時間粗糙度與局部空間運動不連貫性，透過 gamma 修正融合兩種訊號，零參數即可定位操作痕跡。論文並建立服務對齊評估協定，在 ViF-Bench 基準上超越現有 SOTA。

## 核心價值

首個同時支援完整生成影片與局部編輯偵測的零樣本方法，無需微調即可部署於多種生成模型（Sora、Kling、Wan 等）。

## 應用情境與實務影響

為社群媒體、新聞機構與版權平台提供可即時部署的深度偽造影片偵測工具，支援 Sora、Kling、Gen-2 等主流生成模型輸出。

## 補充細節

ECCV 2026 接收論文（32 頁）。作者：J. Hyun, H. Kim。程式碼與資料集已開源。在 Fake Recall @ FPR=0.1% 指標上顯著優於 D3、ReStraV、AIGVDet 等基線。

## 維護紀錄

- 收錄日期：2026-08-06
- 最後更新：2026-08-06

---
title: "D4RT：單一模型實現動態 4D 場景重建，榮獲 CVPR 2026 Best Paper"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-07"
organization: "Google DeepMind / University College London / University of Oxford"
source_url: "https://d4rt-paper.github.io"
date_collected: "2026-10-01"
date_updated: "2026-10-01"
tags:
  - ai
  - paper
---

# D4RT：單一模型實現動態 4D 場景重建，榮獲 CVPR 2026 Best Paper

## 基本資訊

- 發布日期：2026-06-07
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://d4rt-paper.github.io

## 概要

Google DeepMind、UCL 與牛津大學團隊提出 D4RT (Dynamic 4D Reconstruction and Tracking)，以單一統一 Transformer 架構從單一影片同時推斷深度、時空對應與完整相機參數，取代傳統多模型管線（深度、光流、相機位姿分開建模）。核心創新為新穎查詢機制，避免逐幀密集解碼與多任務解碼器管理複雜度，實現高效前向推理。論文從 16,092 篇投稿中脫穎而出，獲 CVPR 2026 Best Paper 榮譽。

## 核心價值

首個以單一前向模型統一解決深度、點追蹤與相機位姿的 4D 重建方法，大幅簡化管線並提升效率，為動態場景理解奠定新基準。

## 應用情境與實務影響

適用於機器人導航、AR/VR 即時重建、自動駕駛動態環境感知等需即時 4D 幾何與運動理解的場景；統一查詢介面降低部署複雜度與計算成本。

## 補充細節

CVPR 2026 於 2026/6/7 落幕，共 16,092 篇投稿、4,089 篇錄取。D4RT 專案頁面：https://d4rt-paper.github.io；開放存取論文與程式碼已釋出。作者包含 Chuhan Zhang、Guillaume Le Moing、Andrew Zisserman、Mehdi Sajjadi 等。

## 維護紀錄

- 收錄日期：2026-10-01
- 最後更新：2026-10-01

---
title: "D4RT：單一模型實現動態 4D 場景重建的 CVPR 2026 最佳論文"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-15"
organization: "Google DeepMind"
source_url: "https://d4rt-paper.github.io"
date_collected: "2026-07-29"
date_updated: "2026-07-29"
tags:
  - ai
  - paper
---

# D4RT：單一模型實現動態 4D 場景重建的 CVPR 2026 最佳論文

## 基本資訊

- 發布日期：2026-06-15
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://d4rt-paper.github.io

## 概要

Google DeepMind、倫敦大學學院與牛津大學團隊在 CVPR 2026 發表 D4RT（Dynamic 4D Reconstruction and Tracking），從超過 16,000 篇投稿中脫穎而出榮獲最佳論文獎。D4RT 以單一統一 Transformer 架構，從單一影片輸入即可同時推測深度、時空對應與完整相機參數，以單次前向傳播取代傳統多模型管線（深度、光流、相機位姿分開估計），實現高效率的動態 4D 重建。

## 核心價值

首個以單一前向傳播模型統一解決動態場景的深度、點追蹤與相機位姿估計，大幅簡化 4D 重建管線並提升效率。

## 應用情境與實務影響

可應用於機器人導航、AR/VR 內容生成、自動駕駛場景理解、數位孿生建構等需即時 4D 幾何與運動理解的場景。專案頁面提供程式碼與示範，方便研究者與工程師快速驗證與二次開發。

## 補充細節

模型編碼器採用 Vision Transformer，重用 VGGT 提出的交錯幀級與全域自注意力機制，將整段影片壓縮為單一全域場景表徵。解碼端透過查詢機制從該表徵按需解碼深度圖、點軌跡與相機參數。在 DAVIS、TAP-Vid、KITTI 等基準上，D4RT 以無優化的單模型超越多階段優化基線。論文已開源於 arXiv:2512.08924，專案頁面 d4rt-paper.github.io 提供模型權重、推論程式碼與互動式 Demo。

## 維護紀錄

- 收錄日期：2026-07-29
- 最後更新：2026-07-29

---
title: "MiMaAlign：階層式微觀-巨觀對齊框架，提升文字生成影片的物理合理性"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-21"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2610.16482"
date_collected: "2026-10-26"
date_updated: "2026-10-26"
tags:
  - ai
  - paper
---

# MiMaAlign：階層式微觀-巨觀對齊框架，提升文字生成影片的物理合理性

## 基本資訊

- 發布日期：2026-10-21
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2610.16482

## 概要

針對現有文字生成影片模型在物理合理性上的不足，提出 MiMaAlign 階層式雙教師對齊框架。結合神經常微分方程（Neural-ODE）學習微觀級連續運動表徵，與指令提示的視覺-語言模型提取的巨觀級事件表徵，透過訓練期輔助目標對齊至生成器不同層級，系統性改善影片生成的物理常識。

## 核心價值

首創微觀運動與巨觀事件雙層級對齊機制，無需推理期額外計算即可跨骨幹模型（CogVideoX、Wan2.1 等）提升物理合理性。

## 應用情境與實務影響

為影片生成模型提供可插拔的對齊範式，適用於內容創作、合成資料生成、世界模型構建等需物理一致性的場景。

## 補充細節

實驗於 VBench-I2V、VideoPhy 等基準達到最高整體品質分數；消融研究證實雙教師信號互補性。作者包括 Yansong Liu、Litong Gong、Weijie Li、Tiezheng Ge、Ming Zeng。

## 維護紀錄

- 收錄日期：2026-10-26
- 最後更新：2026-10-26

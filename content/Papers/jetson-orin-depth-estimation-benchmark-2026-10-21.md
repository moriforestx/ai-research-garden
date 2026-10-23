---
title: "Jetson AGX Orin 上 9 類深度估計模型實測基準：2026 年 10 月最新評測"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-21"
organization: "作者單位未在摘要中明示（arXiv:2610.27199v1）"
source_url: "https://arxiv.org/html/2610.27199v1"
date_collected: "2026-10-24"
date_updated: "2026-10-24"
tags:
  - ai
  - paper
---

# Jetson AGX Orin 上 9 類深度估計模型實測基準：2026 年 10 月最新評測

## 基本資訊

- 發布日期：2026-10-21
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/html/2610.27199v1

## 概要

論文對 Jetson AGX Orin 這類機器人/車載常用邊緣裝置，實測 9 個深度估計模型家族（單目：Depth Anything V2/V3、Depth Pro、MoGe-2、Metric3D v2、UniDepth V2；雙目：libSGM、NVIDIA ESS、Fast-FoundationStereo），全部以 TensorRT FP16 或原生 CUDA 部署，涵蓋準確度、速度、能耗三維指標。

## 核心價值

首次在統一邊緣硬體上給出主流深度模型的全面實測數據，MoGe-2-L 絕對相對誤差 3.8% 領先，Depth Anything V2 Small 僅 11.5 ms 最快。

## 應用情境與實務影響

機器人與自駕團隊可依據準確度/延遲/功耗權衡直接選型，避免自行在目標平台重複基準測試。

## 補充細節

測試解析度最高達 5.7 MP；單目模型在原生輸入下 Depth Anything V2 Small 11.5 ms、Base 26.8 ms、Large 84.5 ms；Depth Pro 全解析度 803 ms；雙目方法 libSGM 12 ms、NVIDIA ESS 8 ms、Fast-FoundationStereo 15 ms。論文指出即使最佳模型仍有 27% 像素誤差超過 5%。

## 維護紀錄

- 收錄日期：2026-10-24
- 最後更新：2026-10-24

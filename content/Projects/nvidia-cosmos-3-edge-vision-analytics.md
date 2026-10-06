---
title: "NVIDIA 發布 Cosmos 3 Edge：4B 參數開放世界基礎模型，邊緣即時視覺分析登頂 VANTAGE-Bench"
type: project
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-20"
organization: "NVIDIA"
source_url: "https://huggingface.co/nvidia/Cosmos3-Edge"
date_collected: "2026-10-07"
date_updated: "2026-10-07"
tags:
  - ai
  - project
---

# NVIDIA 發布 Cosmos 3 Edge：4B 參數開放世界基礎模型，邊緣即時視覺分析登頂 VANTAGE-Bench

## 基本資訊

- 發布日期：2026-07-20
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://huggingface.co/nvidia/Cosmos3-Edge

## 概要

NVIDIA 於 2026 年 7 月 20 日於 Hugging Face 發布 Cosmos 3 Edge，為 40 億參數的緊湊世界基礎模型，採用 mixture-of-transformers 架構可同時處理文字、圖片、影片、環境聲音與物理動作五種模態。模型針對邊緣部署優化，可在 Jetson Thor、RTX PRO、DGX 及 GeForce RTX GPU 上即時推理，權重、推理碼與後訓練配方已開放於 Hugging Face（OpenMDW 1.1 授權）。在 VANTAGE-Bench 視覺分析基準測試中，Cosmos 3 Edge 於同參數級別排名第一。

## 核心價值

首個在單一 GPU 上實現完整物理 AI 管線（感知→推理→動作）的 4B 開放模型，為機器人、自駕車與智慧基礎設施提供即時視覺推理能力。

## 應用情境與實務影響

開發者可直接下載權重於邊緣裝置部署視覺代理，適用於交通監控、公共安全、物流倉儲檢測、工業檢測等固定攝影機場景；也可作為汽車策略模型蒸餾的學生骨幹。Centific、Vaidio 和 YUAN 等廠商已開始評估導入。

## 補充細節

同步發布 VANTAGE-Bench（首個針對真實固定攝影機影像的視覺語言基準）、Traffic Anomaly Reasoning (TAR) 排行榜（AI City Challenge 2026 Track 3 官方榜單）。Cosmos 3 系列另包含 32B Super 與 8B Nano，分別在 VANTAGE-Bench 32B 與 8B 階層領先。蒸餾版 I2V 模型於 Artificial Analysis Image-to-Video 排行榜（2026-07-23）開放權重模型中排名第一。模型採用 OpenMDW 1.1 授權，支援全球部署，並已在 NVIDIA Jetson Thor 平台上驗證可達 15 Hz 實時控制與 32 動作每次推理。

## 維護紀錄

- 收錄日期：2026-10-07
- 最後更新：2026-10-07

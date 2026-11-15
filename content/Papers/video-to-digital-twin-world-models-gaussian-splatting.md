---
title: "從影片到數位孿生：世界模型與高斯濺射在野外影片的探索性研究"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-11-04"
organization: "Robotics Center / Independent"
source_url: "https://arxiv.org/html/2611.10013v1"
date_collected: "2026-11-16"
date_updated: "2026-11-16"
tags:
  - ai
  - paper
---

# 從影片到數位孿生：世界模型與高斯濺射在野外影片的探索性研究

## 基本資訊

- 發布日期：2026-11-04
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/html/2611.10013v1

## 概要

論文探索生成式世界模型與 3D Gaussian Splatting 結合，僅以單一野外走-through 影片（無繪圖、掃描、實地勘測）產出可度量的數位孿生。商業世界模型從 20 幀復原相機位姿與度量深度，融合約 74.7 萬高斯濺射點，成本僅 200 credits（約 0.2 美元）。局部 CPU 優化可達照片級真實，但離拍攝路徑品質快速下降。保留幀 PSNR 達 21.2/23.1 dB（64/43 訓練幀），僅用世界模型接受的 8 幀則下降 3.8/5.4 dB。全流程從首次 commit 到部署後端僅 7 天。

## 核心價值

證明「單一手機級走-through 影片 + 世界模型 + Gaussian Splatting + OpenUSD」即可在極低成本、極短時間產出可互操作的度量級數位孿生，打破傳統需 LiDAR、專業掃描、大量標註的門檻。

## 應用情境與實務影響

設施管理、建築驗收、災害評估、遠端協作等場景可大幅降低 3D 數位化門檻；OpenUSD 輸出可直接接入 Omniverse、Blender、自有資料層。

## 補充細節

作者 Somesh Mohapatra；實驗對象為食物銀行倉庫新聞走-through 影片。使用商業世界模型（未具名）進行相機位姿與深度估計，再以 3DGS 重建。缺口區域以 Blender 程式化建模補齊，輸出 OpenUSD 階層。伺服器無狀態資料層連接既有營運系統。代碼與補充影片已開源。

## 維護紀錄

- 收錄日期：2026-11-16
- 最後更新：2026-11-16

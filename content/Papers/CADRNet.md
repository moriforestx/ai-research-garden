---
title: "CADRNet: Cognitively-Inspired Active Vision for 3D Reasoning Segmentation via Differentiable Rendering"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-01"
authors:
  - "Zai Yang Yu"
  - "Changshuo Wang"
  - "Yuan Shi"
  - "Linjun Sun"
  - "Shu Wei"
  - "Tingran Wang"
  - "Wangyu Wu"
  - "Yanjie Li"
  - "Weijun Li"
keywords:
  - "3D reasoning segmentation"
  - "active vision"
  - "differentiable rendering"
  - "cognitive-inspired"
  - "CVPR 2026"
identifier: "CVPR2026-CADRNet"
identifier_type: "conference"
publication_status: "published"
source_url: "https://openaccess.thecvf.com/content/CVPR2026F/html/Yu_CADRNet_Cognitively-Inspired_Active_Vision_for_3D_Reasoning_Segmentation_via_Differentiable_CVPRF_2026_paper.html"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# CADRNet: Cognitively-Inspired Active Vision for 3D Reasoning Segmentation via Differentiable Rendering

## 基本資訊

- 作者：Zai Yang Yu、Changshuo Wang、Yuan Shi、Linjun Sun、Shu Wei、Tingran Wang、Wangyu Wu、Yanjie Li、Weijun Li
- 發布日期：2026-06-01
- 研究主題：電腦視覺 / Computer Vision
- 關鍵字：3D reasoning segmentation、active vision、differentiable rendering、cognitive-inspired、CVPR 2026
- 論文識別碼：CVPR2026-CADRNet (conference)
- 發表狀態：已發表
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026F/html/Yu_CADRNet_Cognitively-Inspired_Active_Vision_for_3D_Reasoning_Segmentation_via_Differentiable_CVPRF_2026_paper.html

## 摘要

CADRNet 提出一種認知啟發的主動視覺框架，針對 3D 推理分割任務。透過可微渲染機制，模型能夠主動選擇最佳觀測視角，解決語言查詢與幾何表示中存在的歧義。在 3D 推理分割基準上達到 SOTA 表現。

## 核心研究問題

如何讓模型主動獲取最資訊量的視角，以解決 3D 語言引導分割中的幾何與語義歧義？

## 方法與技術

採用認知啟發的主動視覺策略，結合可微渲染器，讓模型在推理過程中預測下一最佳視角。架構包含視覺編碼器、語言編碼器、推理模組與視角選擇策略網路。透過端到端訓練，模型學習主動移動相機以獲取關鍵幾何資訊。

## 實驗與研究結果

在多個 3D 推理分割基準（ScanRefer、Nr3D、Sr3D）上超越既有方法，特別在處理遮擋與歧義場景時表現顯著優於被動視覺基線。

## 研究意義與適用範圍

為具身智能與機器人視覺提供主動感知新範式，適用於需要主動探索環境的 3D 語義理解任務。

## 限制與注意事項

推理階段需要多步視角選擇與渲染，計算成本高於單視角方法；真實機器人部署需解決動態環境下的即時性問題。

## 相關概念

- 3D 推理分割
- 主動視覺
- 可微渲染
- 語言引導分割

## 相關工具與專案

- CVPR 2026 Findings 開放獲取版本

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

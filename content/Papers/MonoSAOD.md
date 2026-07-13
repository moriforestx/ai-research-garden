---
title: "MonoSAOD: Monocular 3D Object Detection with Sparsely Annotated Label"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-15"
authors:
  - "Junyoung Jung"
  - "Seokwon Kim"
  - "Jung Uk Kim"
keywords:
  - "monocular 3D object detection"
  - "sparse annotation"
  - "CVPR 2026"
  - "road-aware patch augmentation"
identifier: "CVPR 2026"
identifier_type: "conference"
publication_status: "published"
source_url: "https://openaccess.thecvf.com/content/CVPR2026/html/Jung_MonoSAOD_Monocular_3D_Object_Detection_with_Sparsely_Annotated_Label_CVPR_2026_paper.html"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# MonoSAOD: Monocular 3D Object Detection with Sparsely Annotated Label

## 基本資訊

- 作者：Junyoung Jung、Seokwon Kim、Jung Uk Kim
- 發布日期：2026-06-15 (CVPR 2026)
- 研究主題：電腦視覺 / Computer Vision
- 關鍵字：monocular 3D object detection、sparse annotation、CVPR 2026、road-aware patch augmentation
- 論文識別碼：CVPR 2026 (conference)
- 發表狀態：已發表
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026/html/Jung_MonoSAOD_Monocular_3D_Object_Detection_with_Sparsely_Annotated_Label_CVPR_2026_paper.html

## 摘要

提出 MonoSAOD，針對稀疏標註的單目 3D 物體偵測。現實場景中完整標註所有物體成本極高，稀疏標註更具實用性。包含兩大核心模組：Road-Aware Patch Augmentation (RAPA) 利用稀疏標註將物體補丁增強到路面區域並保持 3D 幾何一致性；稀疏標註下的幾何一致性損失。

## 核心研究問題

在僅有稀疏 3D 標註的情況下，如何實現高精度的單目 3D 物體偵測？

## 方法與技術

1. **RAPA (Road-Aware Patch Augmentation)**：將已標註物體補丁投影到路面區域，保持 3D 几何一致性，擴充訓練樣本
2. **幾何一致性損失**：在稀疏標註下強制預測與幾何先驗一致
3. **端到端訓練**：單一網路同時輸出 2D/3D 偵測結果

## 實驗與研究結果

在 KITTI 基準上，僅使用 10% 標註資料達到全標註基線 90%+ 表現；在 Waymo Open Dataset 同樣展現優異泛化能力。

## 研究意義與適用範圍

大幅降低 3D 偵測資料標註成本，適用於自駕車、機器人導航等真實部署場景。

## 限制與注意事項

依賴路面幾何先驗，非結構化環境效果待驗證；極度稀疏 (<5%) 時性能下降明顯。

## 相關概念

- 單目 3D 偵測
- 稀疏監督學習
- 資料增強
- 自駕車感知

## 相關工具與專案

- CVPR 2026 Open Access

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

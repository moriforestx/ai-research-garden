---
title: "Steerable Visual Representations"
type: paper
research_topic: "電腦視覺 / Computer Vision"
date_published: "2026-04-02"
date_collected: "2026-07-15"
date_updated: "2026-07-15"
source_url: "https://arxiv.org/abs/2604.02327"
identifier: "arxiv-2604-02327"
tags:
  - ai
  - paper
---

# Steerable Visual Representations

## 基本資訊

- 作者：待補充
- 發布日期：2026-04
- 研究主題：電腦視覺 / Computer Vision
- 關鍵字：Steerable Representations、Visual Representation Learning、ECCV 2026、Equivariance
- 論文識別碼：arXiv:2604.02327
- 發表狀態：Accepted to ECCV 2026
- 主要來源：https://arxiv.org/abs/2604.02327

## 摘要

本文提出 Steerable Visual Representations，一種能夠根據下游任務需求動態調整視覺表示的方法。傳統視覺表示是固定的，而 steerable representations 允許模型在推理階段根據特定任務（如分類、檢測、分割）調整特徵表示。實驗顯示該方法在多個視覺基準測試上優於固定表示基線。

## 核心研究問題

如何學習能夠適應不同下游任務的視覺表示，而不需要為每個任務重新訓練整個模型？

## 方法與技術

1. **Steerable Encoder**：學習一個編碼器，其輸出可以通過可學習的調制參數進行動態調整。
2. **Task-Conditioned Modulation**：引入任務條件向量，控制特徵空間中的旋轉、縮放等幾何變換。
3. **Equivariance Regularization**：通過等變性正則化確保表示在語義保持的前提下具有可控性。
4. **Multi-Task Training**：在多個視覺任務上聯合訓練，學習共享的 steerable 表示空間。

## 實驗與研究結果

- 在 ImageNet 分類、COCO 目標檢測、ADE20K 語義分割等任務上進行評估。
- Steerable representations 在單一模型下超越為各任務單獨訓練的固定表示基線。
- 消融實驗驗證了等變性正則化和任務條件調制的有效性。
- 推理階段計算開銷極小，僅需輕量級調制。

## 研究意義與適用範圍

- 為通用視覺骨幹網絡提供了動態適應能力，減少多任務部署的存儲和計算成本。
- 等變性設計理論扎實，可擴展到 3D 視覺、視頻理解等領域。
- 適合資源受限環境下的多任務視覺應用。

## 限制與注意事項

- 任務條件向量的設計需要領域知識或額外學習。
- 極端任務差異可能導致表示衝突。
- 尚未在大規模預訓練數據集（如 JFT-3B）上驗證擴展性。

## 相關概念

- Equivariant Neural Networks
- Visual Representation Learning
- Multi-Task Learning
- Dynamic Inference

## 相關工具與專案

- 無官方開源代碼倉庫（截至收錄時）

## 維護紀錄

- 收錄日期：2026-07-15
- 最後更新：2026-07-15
- 更新紀錄：
  - 2026-07-15：首次建立

---
title: "RynnBrain: Open Embodied Foundation Models"
type: paper
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-02-13"
authors: []
keywords: []
identifier: "2602.14979"
identifier_type: "arXiv"
publication_status: "preprint"
source_url: "https://arxiv.org/abs/2602.14979"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# RynnBrain: Open Embodied Foundation Models

## 基本資訊

- 作者：RynnBrain 研究團隊
- 發布日期：2026-02-13
- 研究主題：AI 綜合動態 / General AI Updates
- 關鍵字：具身智能、開源基礎模型、時空推理、多模態
- 論文識別碼：2602.14979 (arXiv)
- 發表狀態：預印本
- 主要來源：https://arxiv.org/abs/2602.14979

## 摘要

RynnBrain 是一個開源的時空基礎模型，專為具身智能設計，包含 2B、8B、30B-A3B MoE 三種規模，統一了感知、推理與規劃能力。提供四種後訓練變體（Nav、Plan、VLA、CoP），在 20 個具身基準測試上達到 SOTA 表現。

## 核心研究問題

如何建立一個統一的基礎模型，同時支援機器人導航、任務規劃、視覺語言動作與協作規劃等多樣化具身任務？

## 方法與技術

採用時空注意力架構，結合 MoE 專家混合機制，透過大規模具身數據預訓練，再針對四大下游任務進行專門後訓練。

## 實驗與研究結果

在 20 個具身智能基準測試中均達到最優表現，證明統一架構可有效支援多樣化具身任務。

## 研究意義與適用範圍

為具身智能提供了統一的開源基礎模型選擇，降低多任務整合門檻，適用於機器人導航、操作規劃、視覺語言動作等場景。

## 限制與注意事項

模型參數量大，推理需要較高算力資源；長尾任務表現仍有提升空間。

## 相關概念

- 具身智能
- 基礎模型
- 專家混合架構
- 時空推理

## 相關工具與專案

- RynnBrain Model Zoo
- Embodied Evaluation Suite

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

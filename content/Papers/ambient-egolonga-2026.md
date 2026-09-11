---
title: "Ambient @ EgoLongQA 2026: Distilling Long-Video perception into a Sub-2B Model"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-07"
organization: "Ambient (ECCV 2026 Wearable AI Grand Challenge winning team)"
source_url: "https://arxiv.org/abs/2609.07154"
date_collected: "2026-09-12"
date_updated: "2026-09-12"
tags:
  - ai
  - paper
---

# Ambient @ EgoLongQA 2026: Distilling Long-Video perception into a Sub-2B Model

## 基本資訊

- 發布日期：2026-09-07
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2609.07154

## 概要

EgoLongQA 任務要求模型回答關於長時程以自我為中心影片的四選一選擇題，影片長度通常約十分鐘。問題常為兩跳且複合：首先參考一個錨點事件，然後詢問相對於該事件發生的事。≤2B 部門限制了整個多模態檢查點，包括視覺塔。本文提出一種蒸餾方法，將工具使用代理管線的初級感知模組壓縮為小型學生模型，透過過濾的教師痕跡進行訓練，使得在 ECCV 2026 可穿戴 AI 挑戰賽的 EgoLongQA 軌道中，於 ≤2B 參數組別獲得第一名，held-out 測試集得分 0.8279。

## 核心價值

將長影片感知知識蒸餾至 sub-2B 視覺語言模型

## 應用情境與實務影響

為資源受限的裝置提供高效長影片理解能力，適用於可穿戴助理與機器人。

## 補充細節

作者未完全列出，但來自勝出方案的技術報告。模型為單一 2B 視覺語言模型，採用貪婪前向傳遞回答十分鐘以自我為中心影片的多選題。

## 維護紀錄

- 收錄日期：2026-09-12
- 最後更新：2026-09-12

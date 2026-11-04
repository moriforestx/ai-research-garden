---
title: "SPOD: Recovering Suppressed Temporal Evidence in Video-LLMs via Single-Pass Orthogonal Decomposition"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-11-03"
organization: "arXiv / ACM Multimedia 2026"
source_url: "https://arxiv.org/abs/2611.04728"
date_collected: "2026-11-05"
date_updated: "2026-11-05"
tags:
  - ai
  - paper
---

# SPOD: Recovering Suppressed Temporal Evidence in Video-LLMs via Single-Pass Orthogonal Decomposition

## 基本資訊

- 發布日期：2026-11-03
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2611.04728

## 概要

提出 SPOD（單次正交分解）框架，無需重新訓練即可在單次前向傳播中恢復 Video-LLM 中被抑制的時間證據。包含幀獨特性分析 (FDA) 與時間增量子空間 (TDS) 兩組件，分解隱藏狀態為時間、先驗與殘差分量並獨立重新縮放。

## 核心價值

在 VidHalluc、EventHallusion、VideoMMMU 基準測試上超越強基線，保持近乎原生的推理效率，證明改善時間推理不一定需要額外監督。

## 應用情境與實務影響

解決 Video-LLM 在場景轉換理解、事件排序等時間敏感推理任務中的幻覺問題，免訓練、高效率，易於部署到現有模型。

## 補充細節

作者：Yangguang Lin 等 4 人。arXiv:2611.04728v1，2026-11-03 提交。Accepted to ACM Multimedia 2026 (MM '26)。代碼：https://github.com/VioAgnes/SPOD

## 維護紀錄

- 收錄日期：2026-11-05
- 最後更新：2026-11-05

---
title: "RayRoPE：多視角注意力的投射射線位置編碼"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-03"
organization: "Apple Machine Learning Research"
source_url: "https://machinelearning.apple.com/research/rayrope-projective-ray"
date_collected: "2026-11-27"
date_updated: "2026-11-27"
tags:
  - ai
  - paper
---

# RayRoPE：多視角注意力的投射射線位置編碼

## 基本資訊

- 發布日期：2026-10-03
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://machinelearning.apple.com/research/rayrope-projective-ray

## 概要

Apple 機器學習研究團隊在 ECCV 2026 發表 RayRoPE，提出一種投射射線位置編碼方法，解決多視角注意力機制中的幾何一致性問題。該方法將 3D 射線投射至 2D 特徵圖，為跨視角注意力提供幾何感知的位置先驗，在多視角 3D 重建與深度估計任務上顯著提升效能。論文於 2026 年 9 月 8–12 日在 ECCV 2026（瑞典馬模）發表，論文集於 10 月 3–4 日由 Springer 正式出版。arXiv 預印本於 2026-01-21 提交，2026-07-06 更新至 v3。

## 核心價值

首個將幾何射線投射整合至 Transformer 位置編碼的方法，為多視角視覺任務提供原生 3D 幾何先驗。

## 應用情境與實務影響

改善自動駕駛、機器人導航與 AR/VR 中的多相機系統感知精度，減少跨視角特徵對齊誤差。

## 補充細節

ECCV 2026 論文，作者：Yu Wu, Minsik Jeon, Jen-Hao Rick Chang, Oncel Tuzel, Shubham Tulsiani。會議日期：2026-09-08 至 2026-09-12。論文集電子書出版日期：2026-10-03（ISBN 978-3-032-37419-6）。arXiv:2601.15275v3。專案頁面：https://rayrope.github.io。

## 維護紀錄

- 收錄日期：2026-11-27
- 最後更新：2026-11-27

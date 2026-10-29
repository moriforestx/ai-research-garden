---
title: "360Anything: Geometry-Free Lifting of Images and Videos to 360°"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-08"
organization: "Google DeepMind"
source_url: "https://arxiv.org/abs/2601.16192"
date_collected: "2026-10-30"
date_updated: "2026-10-30"
tags:
  - ai
  - paper
---

# 360Anything: Geometry-Free Lifting of Images and Videos to 360°

## 基本資訊

- 發布日期：2026-09-08
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2601.16192

## 概要

Google DeepMind 發表 360Anything，一個幾何自由的框架，利用預訓練擴散 Transformer 將任意透視圖片與影片提升為無縫、重力對齊的 360° 全景圖，完全不需相機參數或 3D 資訊。該方法在圖像與影片的透視轉 360° 生成任務上達到 SOTA，甚至超越使用真值相機資訊的先前工作。

## 核心價值

證明純資料驅動的幾何自由方法可超越依賴相機校準的傳統方法，為野外資料的全景生成與 3D 場景重建開闢新路徑。

## 應用情境與實務影響

適用於沉浸式 VR/AR 內容生成、機器人環境感知、自動駕駛周邊視覺擴展、以及無相機校準資訊的野外影像全景化。

## 補充細節

ECCV 2026 (2026-09-08 至 2026-09-12，馬爾默)。arXiv:2601.16192v2。作者：Ziyi Wu、Daniel Watson、Andrea Tagliasacchi、David J. Fleet、Marcus A. Brubaker、Saurabh Saxena (Google DeepMind、SFU、UToronto)。專案頁：https://360anything.github.io。核心創新：將透視輸入與全景目標視為 token 序列，以 DiT 學習映射；以圓形潛在編碼解決 ERP 邊界縫合伪影。

## 維護紀錄

- 收錄日期：2026-10-30
- 最後更新：2026-10-30

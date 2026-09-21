---
title: "NitroGen：面向通用遊戲代理的視覺-動作基礎模型"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-01"
organization: "NVIDIA"
source_url: "https://openaccess.thecvf.com/content/CVPR2026/html/Magne_NitroGen_An_Open_Foundation_Model_for_Generalist_Gaming_Agents_CVPR_2026_paper.html"
date_collected: "2026-09-22"
date_updated: "2026-09-22"
tags:
  - ai
  - paper
---

# NitroGen：面向通用遊戲代理的視覺-動作基礎模型

## 基本資訊

- 發布日期：2026-06-01
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026/html/Magne_NitroGen_An_Open_Foundation_Model_for_Generalist_Gaming_Agents_CVPR_2026_paper.html

## 概要

NVIDIA 聯合 Stanford、Caltech、UChicago、UT Austin 等機構在 CVPR 2026 發表 NitroGen，首個在超過 1,000 款遊戲、40,000 小時實況影片上訓練的視覺-動作統一基礎模型。研究構建了自動化管線從公開遊戲影片提取玩家動作，建立跨遊戲泛化基準，採用流匹配擴散架構預測 16 步動作序列，在未見遊戲上較從頭訓練提升 52% 任務成功率。模型權重、資料集、基準環境全數開源。

## 核心價值

首個千遊戲級視覺-動作基礎模型，證明大規模行為克隆可產生跨類型泛化的具身代理，為機器人學與通用代理研究提供可復現基準。

## 應用情境與實務影響

開源模型與資料集直接可用於遊戲 AI、機器人模擬遷移、具身智能預訓練；自動化動作提取管線可擴展至其他視頻數據源。

## 補充細節

架構採用 SigLIP-2 視覺編碼器 (256×256) + 擴散 Transformer，流匹配生成動作塊。CVPR 2026 Oral 發表，Best Paper Honorable Mention。arXiv:2601.02427。Hugging Face: nvidia/NitroGen。專案頁: nitrogen.minedojo.org。

## 維護紀錄

- 收錄日期：2026-09-22
- 最後更新：2026-09-22

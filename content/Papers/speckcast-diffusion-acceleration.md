---
title: "SpecKCast：以譜域卡爾曼預測加速擴散變換器推理"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-20"
organization: "University of Toronto / Vector Institute / Samsung Electronics AI Center Toronto"
source_url: "https://arxiv.org/abs/2610.26837"
date_collected: "2026-10-22"
date_updated: "2026-10-22"
tags:
  - ai
  - paper
---

# SpecKCast：以譜域卡爾曼預測加速擴散變換器推理

## 基本資訊

- 發布日期：2026-10-20
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2610.26837

## 概要

多倫多大學、Vector Institute 與三星電子多倫多 AI 中心研究者提出 SpecKCast，一種無需訓練的擴散變換器推理加速方法。該方法在頻域以卡爾曼濾波追蹤特徵係數的時序動態，預測下一步係數以跳過部分去噪步驟。在 FLUX 等最先進生成模型上測試，SpecKCast 最高達 6× 加速，且記憶體開銷極小，優於現有快取與係數預測基線。

## 核心價值

展示在頻域建模擴散軌跡可大幅減少推理步數而不損畫質，為生成式視覺模型部署提供實用的免訓練加速路徑。

## 應用情境與實務影響

適用於需低延遲生成的應用（即時圖像/視頻編輯、互動式設計工具），可直接整合至現有 DiT 推理管線，無需重新訓練或微調。

## 補充細節

論文編號：arXiv:2610.26837 (cs.CV)，2026-10-20 提交。作者：Javad Rajabi、Hakki Can Karaimer、David B. Lindell、Babak Taati、Michael S. Brown。核心貢獻：(1) 將擴散變換器的特徵演化視為頻域中的線性動態系統；(2) 以卡爾曼濾波器線上估計並預測頻譜係數；(3) 依預測信心動態決定跳過步數；(4) 在 FLUX.1-dev、SD3 等模型上驗證，FID/CLIP 分值基本持平下實現 2–6× 加速。

## 維護紀錄

- 收錄日期：2026-10-22
- 最後更新：2026-10-22

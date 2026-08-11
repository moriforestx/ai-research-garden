---
title: "In Pursuit of Pixel Supervision for Visual Pre-training"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-19"
organization: "Meta FAIR"
source_url: "https://openaccess.thecvf.com/content/CVPR2026/html/Yang_In_Pursuit_of_Pixel_Supervision_for_Visual_Pre-training_CVPR_2026_paper.html"
date_collected: "2026-08-12"
date_updated: "2026-08-12"
tags:
  - ai
  - paper
---

# In Pursuit of Pixel Supervision for Visual Pre-training

## 基本資訊

- 發布日期：2026-06-19
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026/html/Yang_In_Pursuit_of_Pixel_Supervision_for_Visual_Pre-training_CVPR_2026_paper.html

## 概要

Meta FAIR、HKU、NYU 與 MIT 團隊提出 PIXO，一個純粹以像素預測作為監督訊號的自監督視覺預訓練模型。基於 MAE 架構，透過更深解碼器、大塊遮罩與額外類別標記增強，於 20 億網路爬取圖片上以自策展策略訓練。PIXO 在單目深度估計、前饋 3D 重建、物件分割與具身 AI 等下游任務表現優異，證明像素級監督即可學習豐富視覺屬性，同時保持簡單、穩定且高效。此為 CVPR 2026 Highlight 論文。

## 核心價值

證明大規模像素級自監督預訓練無需語義標註即可學得強韌視覺表示，重新定義視覺預訓練的監督範式。

## 應用情境與實務影響

為深度估計、3D 重建、分割與機器人學提供統一預訓練基座；模型與代碼將公開釋出，加速下游應用開發。

## 補充細節

作者：Lihe Yang、Shang-Wen Li、Yang Li、Xinjie Lei、Dong Wang、Abdelrahman Mohamed、Saining Xie、Hengshuang Zhao、Kaiming He、Hu Xu。隸屬：FAIR Meta、HKU、NYU、MIT。arXiv：2512.15715（2025-12 發布），CVPR 2026 正式發表於 2026-06。專案頁面：https://pixo.fair.ai/。CVPR 開放存取頁面：https://openaccess.thecvf.com/content/CVPR2026/html/Yang_In_Pursuit_of_Pixel_Supervision_for_Visual_Pre-training_CVPR_2026_paper.html

## 維護紀錄

- 收錄日期：2026-08-12
- 最後更新：2026-08-12

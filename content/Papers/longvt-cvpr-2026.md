---
title: "LongVT：透過原生工具呼叫實現「長影片思考」的端到端代理框架 (CVPR 2026)"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-01"
organization: "EvolvingLMMs-Lab (多機構合作)"
source_url: "https://openaccess.thecvf.com/content/CVPR2026/papers/Yang_LongVT_Incentivizing_Thinking_with_Long_Videos_via_Native_Tool_Calling_CVPR_2026_paper.pdf"
date_collected: "2026-11-19"
date_updated: "2026-11-19"
tags:
  - ai
  - paper
---

# LongVT：透過原生工具呼叫實現「長影片思考」的端到端代理框架 (CVPR 2026)

## 基本資訊

- 發布日期：2026-06-01
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://openaccess.thecvf.com/content/CVPR2026/papers/Yang_LongVT_Incentivizing_Thinking_with_Long_Videos_via_Native_Tool_Calling_CVPR_2026_paper.pdf

## 概要

LongVT 針對大型多模態模型 (LMM) 處理長影片時產生幻覺、難以定位稀疏時序證據的問題，提出首個端到端代理框架，透過交錯多模態工具鏈思維 (iMCoTT) 實現「長影片思考」。模型利用內建的時序定位能力作為原生 `crop_video` 工具，先全域預覽再按需擷取細粒度片段，反覆推理直到答案落在視覺證據上。作者構建 VideoSIAH 基準與資料套件，三階段訓練 (SFT → RL → 微調) 後，LongVT 在長影片問答、時序定位等任務顯著優於基線，並釋出開源代碼與模型。

## 核心價值

首創將 LMM 內建定位能力轉化為可微工具鏈，讓模型像人類「略讀→細讀」般處理時長數小時影片，開啟代理式長影片推理新範式。

## 應用情境與實務影響

適用於長會議紀錄分析、監控影片檢索、影片問答系統等需跨越時序推理的場景；開源模型與 VideoSIAH 基準可直接用於後續研究與產品化落地。

## 補充細節

論文於 2026-02-21 獲 CVPR 2026 接收，arXiv v3 更新於 2026-05-21，CVPR 2026 大會約於 2026-06 中舉行；官方專案頁 https://evolvinglmms-lab.github.io/LongVT、GitHub https://github.com/EvolvingLMMs-Lab/LongVT、arXiv https://arxiv.org/abs/2511.20785。

## 維護紀錄

- 收錄日期：2026-11-19
- 最後更新：2026-11-19

---
title: "Kandinsky 6.0 Video：同步視訊與音訊生成的開源基礎擴散模型"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-04"
organization: "Kandinsky Lab"
source_url: "https://arxiv.org/abs/2610.05608"
date_collected: "2026-10-12"
date_updated: "2026-10-12"
tags:
  - ai
  - tool
---

# Kandinsky 6.0 Video：同步視訊與音訊生成的開源基礎擴散模型

## 基本資訊

- 發布日期：2026-10-04
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2610.05608

## 概要

Kandinsky 團隊發布 Kandinsky 6.0 Video，包含兩個開源基礎擴散模型：Kandinsky 6.0 Video Lite（3B 參數）與 Kandinsky 6.0 Video Pro（29B 參數）。兩模型皆支援 5 秒視訊片段生成，並同步輸出 44 kHz 音訊（含唇形同步），支援文字生成視訊音訊（T2AV）與圖片生成視訊音訊（I2AV）模式；內建超解析度模型可將輸出提升至 Full-HD（1920×1080）。架構採用雙流 CrossDiT，將預訓練視訊流與新訓練音訊流透過雙向交叉注意力機制連接，以達成時間與語義對齊。採持續預訓練策略：先於大規模音訊語料訓練音訊流，再於配對視訊音訊資料聯合訓練，接著進行監督式微調、強化學習後訓練與蒸餾。人工側評顯示 Pro 版優於前代 Kandinsky 5.0 Video Pro，且在語音品質上與領先視訊音訊生成模型具競爭力。代碼、模型權重與 diffusers 整合以 MIT 開源授權釋出。

## 核心價值

開源同步視訊音訊生成基礎模型，雙流 CrossDiT 架構實現高品質唇形同步，MIT 授權釋出模型權重與部署工具，降低多媒體生成研究門檻。

## 應用情境與實務影響

為開源社群提供可直接部署的高品質 T2AV/I2AV 模型，支援 Full-HD 輸出與 44 kHz 音訊，適用於內容創作、虛擬主播、無障礙媒體生成等場景；強化學習後訓練與蒸餾流程亦為後續模型優化提供參考。

## 補充細節

提交日期：2026-10-04 (v1)。模型權重與代碼：https://github.com/kandinskylab/kandinsky-6。授權：MIT。兩模型變體：Lite (3B) 與 Pro (29B)。輸出：5 秒視訊 + 44 kHz 音訊。解析度：內建超解析至 1920×1080。架構：雙流 CrossDiT + 雙向交叉注意力。訓練流程：音訊流預訓練 → 聯合預訓練 → SFT → RL 後訓練 → 蒸餾。

## 維護紀錄

- 收錄日期：2026-10-12
- 最後更新：2026-10-12

---
title: "Can Agents Generalize to the Open World? Unveiling the Fragility of Static Training in Tool Use"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-07-01"
organization: "Nanjing University / LAMDA-NeSy Lab"
source_url: "https://arxiv.org/abs/2607.01084"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - paper
---

# Can Agents Generalize to the Open World? Unveiling the Fragility of Static Training in Tool Use

## 基本資訊

- 發布日期：2026-07-01
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2607.01084

## 概要

Lv 等人於 2026 年 7 月 1 日提交至 ICML 2026 並獲接收的論文（arXiv:2607.01084），系統性探討 LLM 代理人在開放世界工具使用中的泛化能力。研究定義 OpenAgent 問題設定，將環境分佈偏移分為查詢、動作、觀察、領域四大維度，並在可控沙箱中建立四層次（感知、交互、推理、內化）的細粒度偏移基準。實驗表明，無論採用監督微調（SFT）或強化學習（RL）訓練的代理人，面對開放世界分佈偏移均會出現不同程度的效能下降。基於此提出 Perturbation-Augmented Fine-Tuning（擾動增強微調），在 SFT 階段注入多樣化干擾，顯著提升代理人在未見工具、新任務類型與噪聲觀測下的穩健性。代碼開源於 GitHub。

## 核心價值

首次以四層次分類法系統量測工具使用代理人在開放世界分佈偏移下的泛化斷層，並提出低成本的擾動增強 SFT 策略，為實際部署環境下的代理人穩健性提供可驗證基準與改進方向。

## 應用情境與實務影響

代理人開發團隊可直接採用論文開源的沙箱環境與評測協議，在部署前系統性壓測模型對工具集變更、參數分佈漂移、觀察噪聲等真實世界偏移的耐受度；Perturbation-Augmented Fine-Tuning 只需在現有 SFT 流程中加入擾動採樣，即可大幅降低線上故障率。

## 補充細節

作者：Song-Lin Lv、Weiming Wu、Rui Zhu、Zi-Jian Cheng、Lan-Zhe Guo（南京大學 LAMDA-NeSy 實驗室）。論文已被 ICML 2026 接收。實驗基於 8 個基礎模型（Llama-3.1-8B-Instruct 等），對比 SFT、RL、Perturbation-Augmented SFT 三種訓練範式，在 12 類分佈偏移下累計 2.4 萬輪交互。代碼與數據將釋出於 https://github.com/LAMDA-NeSy/OpenAgent。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

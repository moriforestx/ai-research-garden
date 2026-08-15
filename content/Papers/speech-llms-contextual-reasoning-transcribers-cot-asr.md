---
title: "Speech LLMs are Contextual Reasoning Transcribers：引入思維鏈推理的語音辨識新範式"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-04-01"
organization: "Microsoft Core AI"
source_url: "https://arxiv.org/abs/2604.00610"
date_collected: "2026-08-15"
date_updated: "2026-08-15"
tags:
  - ai
  - paper
---

# Speech LLMs are Contextual Reasoning Transcribers：引入思維鏈推理的語音辨識新範式

## 基本資訊

- 發布日期：2026-04-01
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2604.00610

## 概要

Microsoft Core AI 團隊提出 CoT-ASR（Chain-of-Thought ASR），讓大型語言模型在語音辨識過程中先產生情境推理鏈，再輸出逐字稿。透過 CTC non-blank token 機率加權 LLM embedding 的 CTC-weighted LLM Adapter，有效對齊語音編碼器輸出與 LLM 文字潛在空間。實驗顯示相較標準 LLM-based ASR，CoT-ASR 字錯率 (WER) 相對降低 8.7%、實體錯誤率 (EER) 相對降低 16.9%，並在語音翻譯、口語問答等下游任務展現泛化能力。

## 核心價值

首次將思維鏈推理引入端到端語音辨識，證明 LLM 內建的生成式推理能力可顯著提升 ASR 準確度，特別是實體識別等需語境理解的場景。

## 應用情境與實務影響

語音助理、會議紀錄、醫療口述等對專有名詞準確度敏感的應用可直接受益；CTC-weighted Adapter 為無需重新訓練語音編碼器即可接入新 LLM 提供實作路徑。

## 補充細節

論文編號 arXiv:2604.00610v1（2026-04-01 提交），作者：Keqi Deng、Ruchao Fan、Bo Ren、Yiming Wang、Jinyu Li（Microsoft Core AI）。CoT-ASR 透過三階段生成：(1) 語境分析、(2) 實體預測、(3) 逐字稿輸出。在 LibriSpeech、GigaSpeech、內部多語言資料集驗證。程式碼與模型將開源於 Microsoft Research GitHub。Microsoft Research 專頁：https://www.microsoft.com/en-us/research/publication/speech-llms-are-contextual-reasoning-transcribers。

## 維護紀錄

- 收錄日期：2026-08-15
- 最後更新：2026-08-15

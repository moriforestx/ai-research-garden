---
title: "VeriSpoof: Beyond Real or Fake with One Audio LLM"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-11-04"
organization: "University of Melbourne"
source_url: "https://arxiv.org/abs/2611.04634"
date_collected: "2026-11-12"
date_updated: "2026-11-12"
tags:
  - ai
  - paper
---

# VeriSpoof: Beyond Real or Fake with One Audio LLM

## 基本資訊

- 發布日期：2026-11-04
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2611.04634

## 概要

提出 VeriSpoof，一個開放權重的音頻語言模型，統一五項語音偽造檢測任務：深度偽造檢測、生成器歸因、錄製條件分析、合成片段定位、來源驗證。基於 Qwen3-ASR-1.7B 音頻編碼器與 MiniCPM5-2B 語言模型，僅訓練 29.7M 參數，支援可驗證的推理輸出。

## 核心價值

單一模型統一五大語音取證任務，提供可檢核的推理過程，能捕捉單一分數遺漏的部分偽造，並在未見過的編輯類型下保持高準確度。

## 應用情境與實務影響

語音深度偽造檢測、數位取證、內容驗證平台、媒體審核等場景直接受益；開放模型與基準測試（VeriSpoof-Bench）促進領域發展。

## 補充細節

作者：Yang Xiao、Ting Dang（墨爾本大學）。arXiv:2611.04634v1，2026年11月4日發布。模型 2.85B 參數，LoRA (r=16, α=32) 適配，單張 24GB GPU 可訓練。發布 VeriSpoof-Base、VeriSpoof-Plus、VeriSpoof-Plus-MLX-8bit 三個版本。在 Speech-DF-Arena 14 個測試集上排名第一。

## 維護紀錄

- 收錄日期：2026-11-12
- 最後更新：2026-11-12

---
title: "Φ-Bench: Can Large Language Models Engineer the Infrastructure That Powers Them?"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-15"
organization: "USTC, StepFun, PKU, HKUST, Yale, UPenn"
source_url: "https://arxiv.org/abs/2609.10226"
date_collected: "2026-11-08"
date_updated: "2026-11-08"
tags:
  - ai
  - paper
---

# Φ-Bench: Can Large Language Models Engineer the Infrastructure That Powers Them?

## 基本資訊

- 發布日期：2026-10-15
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2609.10226

## 概要

來自 USTC、StepFun、PKU、HKUST、Yale、UPenn 等機構的 Φ-Bench 基準，專門測試前沿 LLM 與編碼代理在真實 LLM 基礎設施工程任務上的表現。包含 85 個自包含、Docker 可復現任務，涵蓋 GPU/CUDA 核心優化、分散式訓練、推理服務 (vLLM)、低精度量化、通訊集合、檢查點存儲、MoE 路由、注意力與狀態空間核心。實驗顯示最強模型 Claude Opus 5 僅得 36.53%，且所有模型在長視野、倉庫級實作任務上表現顯著遜於核心級任務。

## 核心價值

首個系統性評估 LLM 自我工程化基礎設施能力的基準，揭示當前模型在長視野、開放式系統工程任務上的嚴重不足。

## 應用情境與實務影響

為 LLM 基礎設施自動化研發提供量化基線；凸顯代理式編碼在系統層面的缺口，指導後續模型訓練與代理設計；開源任務套件、評分器與參考解可直接納入 CI/CD 驗證管線。

## 補充細節

論文編號 arXiv:2609.10226v2，分類 cs.CL。作者群包含 Shumin Wang、Yiming Xu、Feiyuan Zhang 等。任務分三類：KFC（核心函數完成）、LH（長視野實作）、E2E（端到端優化）。代碼開源於 GitHub (one2piece2hello/faibench_Frontier_InfraBench)，數據集發布於 Hugging Face，官網 faibench.org。

## 維護紀錄

- 收錄日期：2026-11-08
- 最後更新：2026-11-08

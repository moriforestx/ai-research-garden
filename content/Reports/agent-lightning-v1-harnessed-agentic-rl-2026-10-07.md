---
title: "Agent Lightning v1.0：微軟亞洲研究院推出 3,500 行輕量級代理人 RL 框架"
type: report
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-10-07"
organization: "Microsoft Research"
source_url: "https://www.microsoft.com/en-us/research/blog/agent-lightning-v1-0-a-3500-line-lightweight-agentic-rl-framework-for-training-agents-with-real-harnesses"
date_collected: "2026-10-26"
date_updated: "2026-10-26"
tags:
  - ai
  - report
---

# Agent Lightning v1.0：微軟亞洲研究院推出 3,500 行輕量級代理人 RL 框架

## 基本資訊

- 發布日期：2026-10-07
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://www.microsoft.com/en-us/research/blog/agent-lightning-v1-0-a-3500-line-lightweight-agentic-rl-framework-for-training-agents-with-real-harnesses

## 概要

微軟亞洲研究院發布 Agent Lightning v1.0，一個約 3,500 行程式碼的輕量級 Harnessed Agentic RL 框架。核心創新在於讓部署時使用的代理人 Harness 直接參與強化學習訓練，無需在訓練框架中重新實作代理人。支援任意代理人 Harness，在指令追隨、搜尋、編碼代理人上驗證。實驗顯示：僅用 6K 訓練樣本與適度算力，RL 將 Qwen3.5-9B 在 SWE-bench Verified 上從 41.8% 提升至 56.4%（絕對增益 14.6 點）。框架已開源，三大核心組件：API Gateway、Rollout Controller、Customized Trainer。

## 核心價值

首創「Harnessed Agentic RL」範式：部署時的 Harness 直接參與 RL 訓練，消除訓練與部署環境不一致問題；極簡架構降低進入門檻，推動代理人 RL 實用化。

## 應用情境與實務影響

為代理人開發者提供輕量、可擴充的 RL 訓練基礎設施；加速中小型模型（如 9B 級）在程式碼生成、工具使用等任務上的能力對齊。

## 補充細節

已被 verl Uni-Agent、AReaL 2.0、slime、Polar 等框架採用。技術報告：arXiv:2608.17528。Hugging Face 論文頁：2608.17528。作者單位：Microsoft Research Asia。

## 維護紀錄

- 收錄日期：2026-10-26
- 最後更新：2026-10-26

---
title: "持續改進與並行自主探索：面向大規模解空間的 LLM-Agent 框架"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-08-04"
organization: "Mercari, Inc."
source_url: "https://arxiv.org/abs/2608.04341"
date_collected: "2026-08-15"
date_updated: "2026-08-15"
tags:
  - ai
  - paper
---

# 持續改進與並行自主探索：面向大規模解空間的 LLM-Agent 框架

## 基本資訊

- 發布日期：2026-08-04
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2608.04341

## 概要

Mercari 研究團隊提出一個雙機制 LLM-Agent 框架：(1) 持續改進獎勵迴路——以保留測試集排行榜分數為獎勵信號，驅動單一 Agent 反覆優化提交方案；(2) 並行自主探索底層——支援多 Agent 全自主並行搜尋大規模解空間，無需人工介入。於產品目錄匹配任務實證：單 Agent 合格覆蓋率 47.8–57.4%，五 Agent 並行提升至 62.8–69.4%，顯著超越 33.3% 基線。論文獲接收於 ACM KDD'26 Workshop on SciSoc Agents & LLMs（2026 年 8 月、濟州島）。

## 核心價值

首個將「保留測試集排行榜」形式化為 Agent 內在獎勵信號的框架，證明並行自主探索能發現質化不同的解決方案，為科學發現與工程優化任務提供可復現的自主搜尋基礎設施。

## 應用情境與實務影響

電商目錄匹配、藥物分子優化、晶片佈局搜尋等大規模離散優化問題，可直接套用此框架部署自主 Agent 群，無需人工設計獎勵函數或監督訓練資料。

## 補充細節

論文編號 arXiv:2608.04341v1（2026-08-04 提交），作者：Dulmini Hettiarachchi、Andre Rusli、Julio Christian Young、Sho Akiyama（均屬 Mercari, Inc. Japan）。框架包含：Leaderboard Evaluator（保留測試集評分）、Agent Controller（迭代提示與方案生成）、Parallel Orchestrator（多 Agent 調度與去重）。實驗基準為 Mercari 內部產品目錄匹配資料集（超過 10 萬類別）。程式碼將開源於 Mercari GitHub。

## 維護紀錄

- 收錄日期：2026-08-15
- 最後更新：2026-08-15

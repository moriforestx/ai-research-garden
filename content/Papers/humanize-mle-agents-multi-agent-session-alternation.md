---
title: "Humanize MLE Agents: Multi-Agent Session Alternation Beyond Single-Agent Limits"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-10-09"
organization: "N/A"
source_url: "https://arxiv.org/abs/2610.13494"
date_collected: "2026-10-14"
date_updated: "2026-10-14"
tags:
  - ai
  - paper
---

# Humanize MLE Agents: Multi-Agent Session Alternation Beyond Single-Agent Limits

## 基本資訊

- 發布日期：2026-10-09
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2610.13494

## 概要

提出 Humanize MLE Agents (HMA) 架構，透過兩個代理人在共享工作空間交替運作、限制每階段最多 k 次實驗並重置上下文，無需額外任務專用工具或先驗知識。在 MLE-bench 75 個 Kaggle 任務上達到 78.2% any-medal 率，超越最強開源基線 8.0 個百分點，且僅花費其 1/4 時間預算。證明多代理人交替會話能突破單代理人上下文窗口與錯誤累積限制。

## 核心價值

首個在 MLE-bench 達到 SOTA 的輕量級多代理人協作架構，以會話交替機制解決長程任務中的上下文爆炸與錯誤傳播，代碼開源且無需任務特化工程。

## 應用情境與實務影響

自動化機器學習工程、Kaggle 競賽代理、程式碼生成與除錯代理、長程任務代理架構設計參考。

## 補充細節

arXiv:2610.13494v1，發布於 2026-10-09。作者來自多機構合作（含 Song Han、Sihao Liu、Ligeng Zhu 等）。HMA 核心機制：Solve Agent 執行實驗、Review Agent 檢視結果並規劃下一階段，交替進行並定期重置上下文。實驗涵蓋表格、影像、文本等多模態任務。代碼見論文連結。

## 維護紀錄

- 收錄日期：2026-10-14
- 最後更新：2026-10-14

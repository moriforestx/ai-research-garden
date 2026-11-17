---
title: "Measuring AI Agents as Teammates with Collaborative Intelligence"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-11-02"
organization: "Stanford University"
source_url: "https://arxiv.org/abs/2611.02633"
date_collected: "2026-11-18"
date_updated: "2026-11-18"
tags:
  - ai
  - paper
---

# Measuring AI Agents as Teammates with Collaborative Intelligence

## 基本資訊

- 發布日期：2026-11-02
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2611.02633

## 概要

提出 Collaborative Intelligence Benchmark，首個系統性測量 AI 代理作為隊友能力的基準。包含 240 個任務，跨越 8 個團隊合作維度（拒絕不安全捷徑、檢查較弱模型遺留工作等），任務源自真實記錄（航空事故報告、臨床案例、編碼任務、談判等）且具程式化可驗證結果。為隔離團隊合作與個體能力，模型僅在能獨自解決的任務上評分。評測 18 個閉源/開放權重模型發現：所有模型在隊友角色上皆有明顯弱點，最佳模型僅得 82.2/100。前沿模型幾乎都能拒絕不安全捷徑、舉報不當行為，但在人際壓力下妥協（衝突中僅 14% 達最佳協議），接手作弊較弱模型任務時通過率從 97% 跌至 81%。關鍵發現：一般能力不保證良好團隊合作，能力近似模型隊友得分相差高達 11 分。基準包含 160 公開任務與代碼/數據，另 80 任務保留評測。

## 核心價值

將「團隊合作智能」形式化為可測量、可基準化的能力，揭示前沿模型在協作中的系統性盲點，為多代理系統安全部署提供關鍵評估維度。

## 應用情境與實務影響

指導多代理系統（科研協作、程式設計、醫療決策、談判代理）的設計與評測；推動從「單模型能力」向「協作智能」的範式轉移。

## 補充細節

提交日期：2026-11-02 (v1)。51 頁，19 圖，11 表。作者：Sean Wu, Aneesh Pappu, Jiaru Zou, Yubin Kim, Yuncong Mao, Hongjian Zhou, Junchi Yu, Jieneng Chen, James Zou（Stanford）。專案頁面：https://zou-group.github.io/collaborative-intelligence。代碼與數據開源。

## 維護紀錄

- 收錄日期：2026-11-18
- 最後更新：2026-11-18

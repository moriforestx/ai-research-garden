---
title: "AgentWorld: Benchmarking Long-Horizon Collaboration of Multi-agent LLMs"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-09-25"
organization: "Columbia University, UPenn, Seoul National University, Penn State University"
source_url: "https://arxiv.org/abs/2609.31590"
date_collected: "2026-10-28"
date_updated: "2026-10-28"
tags:
  - ai
  - paper
---

# AgentWorld: Benchmarking Long-Horizon Collaboration of Multi-agent LLMs

## 基本資訊

- 發布日期：2026-09-25
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2609.31590

## 概要

提出 AgentWorld 基準測試，專門評估多 LLM 代理在長時程（50+ 互動輪次）、非對稱角色、黑盒環境下的真實協作能力。建構於支援 1,000 並發代理的 MMORPG 沙箱，包含 100 個人工標註任務（含 100 擴增變體），需 3-20 代理透過自然語言協作。引入因果協作效力指標，量化團隊貢獻而非單純成功率。最強模型僅完成約半數任務，揭示現有代理在長程協作上的顯著缺口。

## 核心價值

填補多代理基準測試長期缺乏「長時程、非對稱角色、黑盒協作」評估維度的空白，提供可復現的 MMORPG 環境與因果度量標準。

## 應用情境與實務影響

為多代理系統研發提供標準化壓力測試場景；代碼與數據開源，可直接用於代理協作機制改進、通訊協議設計、角色分工學習等研究。

## 補充細節

arXiv:2609.31590v1 [cs.MA]，提交日期 2026-09-25，接受於 COLM 2026。作者：Yusen Zhang、Yuan Yuan、Wenliang Zheng、Sharath Chandra Guntuku、Lyle Ungar、Zhou Yu、Rui Zhang 等（Columbia、UPenn、Seoul National、Penn State 等機構）。專案網站與代碼已發布。模擬器提供 380+ 物品、144 怪物類型、70+ NPC、13 高階 API 工具。

## 維護紀錄

- 收錄日期：2026-10-28
- 最後更新：2026-10-28

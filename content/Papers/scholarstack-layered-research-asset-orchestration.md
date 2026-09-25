---
title: "ScholarStack: Layered Research Asset Orchestration and Cross-Task Reuse for Scientific Agents"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-09-20"
organization: "ScholarSeed AI Team"
source_url: "https://arxiv.org/abs/2609.23735"
date_collected: "2026-09-26"
date_updated: "2026-09-26"
tags:
  - ai
  - paper
---

# ScholarStack: Layered Research Asset Orchestration and Cross-Task Reuse for Scientific Agents

## 基本資訊

- 發布日期：2026-09-20
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2609.23735

## 概要

ScholarSeed AI Team 提出 ScholarStack，針對科學研究代理人重複檢索、難以跨任務復用理解的問題，建立分層研究資產框架：將論文集編譯為可版本化、可復用的 L1–L3 知識視圖（原始片段→結構化主張→綜合細論），支援檢索、問答、證據生成、聲明評估等多任務。在 ReportBench-ML 25 任務與 NLPCC 2026 聲明評估基準上，較基線大幅降低 Token 成本並提升準確率。

## 核心價值

將科學代理人從「單任務工具」升級為「資產導向工作流」，以結構化知識資產實現跨任務理解復用，大幅提升效率與一致性。

## 應用情境與實務影響

適用於文獻綜述自動化、研究假設生成、專利分析、系統性證據綜合等需長期、多輪、跨任務的科學研究場景，降低重複計算與幻覺風險。

## 補充細節

arXiv:2609.23735v1，發布 2026-09-20。作者：ScholarSeed AI Team、Ao Zhang、Caoqinwei Gong 等 21 位。核心架構：三層資產（L1 原始片段、L2 結構化主張、L3 綜合細論）、版本化資產庫、任務無關編譯管線、技能模組化（檢索、綜述、評估）。實驗：ReportBench-ML 25 任務對比 PaperQA、OpenScholar、STORM，Token 降低 40%+ 且覆蓋率更高；NLPCC 2026 聲明評估 8080 樣本，準確率領先全文基線。代碼與資產開源。

## 維護紀錄

- 收錄日期：2026-09-26
- 最後更新：2026-09-26

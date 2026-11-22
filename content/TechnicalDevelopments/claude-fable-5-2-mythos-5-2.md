---
title: "Anthropic 發布 Claude Fable 5.2 與 Claude Mythos 5.2"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-11-09"
organization: "Anthropic"
source_url: "https://www.anthropic.com/claude-fable-and-mythos-5-2"
date_collected: "2026-11-23"
date_updated: "2026-11-23"
tags:
  - ai
  - technical-development
---

# Anthropic 發布 Claude Fable 5.2 與 Claude Mythos 5.2

## 基本資訊

- 發布日期：2026-11-09
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://www.anthropic.com/claude-fable-and-mythos-5-2

## 概要

Anthropic 於 2026-11-09 正式發布 Claude Fable 5.2 與 Claude Mythos 5.2，為其最強大的技術工作模型，在程式碼撰寫、金融分析與科學研究領域建立新標竿。Fable 5.2 為公開可用的 Mythos 級模型，Mythos 5.2 則針對防禦性網路安全工作流提供給驗證合作夥伴。兩模型輸出速度較 5.1 版提升 30%，定價降為 $8/百萬輸入 token、$40/百萬輸出 token，並提供可選快速模式（最快 2.5 倍）。Fable 5.2 在 CyScenarioBench 發現漏洞率比 Opus 5.5 高 10.2%、比 Mythos 5.1 高 14.4%；Mythos 5.2 判斷力與校準度顯著改善，測試中無誇大嚴重性的情況。支援 1M token 上下文窗口、128K 最大輸出、自適性思考（永開）、預設 high effort、知識截止 2026-06。

## 核心價值

Mythos 級能力以更低價格、更快速度對外開放，Fable 5.2 為 95% 專業用例提供同等效能，高風險領域透過能力路由導向 Opus 4.8

## 應用情境與實務影響

大型軟體工程（多倉庫、單一巨型倉庫）、金融建模、科學研究、防禦性網路安全審計；快速模式適用於即時互動場景；批次 API 提供 50% 折扣

## 補充細節

系統卡詳述評估方法。Fable 5.2 透過 Claude API 以 `claude-fable-5-2` 存取。Mythos 5.2 僅限網路安全驗證計畫與生物化學研究者。定價：標準 $8/$40，快速模式 $16/$80。知識截止 2026-06。同步宣布 AI for Science 計畫擴展至 20 科學基金會與研究機構。

## 維護紀錄

- 收錄日期：2026-11-23
- 最後更新：2026-11-23

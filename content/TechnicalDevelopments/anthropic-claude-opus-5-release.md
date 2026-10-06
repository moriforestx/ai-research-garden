---
title: "Anthropic 發布 Claude Opus 5：半成本接近 Fable 5 前沿智能的日常旗艦模型"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-07-24"
organization: "Anthropic"
source_url: "https://venturebeat.com/ai/anthropic-launches-claude-opus-5-a-cheaper-ai-model-for-coding-agents-and-enterprise-workflows"
date_collected: "2026-10-07"
date_updated: "2026-10-07"
tags:
  - ai
  - technical-development
---

# Anthropic 發布 Claude Opus 5：半成本接近 Fable 5 前沿智能的日常旗艦模型

## 基本資訊

- 發布日期：2026-07-24
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://venturebeat.com/ai/anthropic-launches-claude-opus-5-a-cheaper-ai-model-for-coding-agents-and-enterprise-workflows

## 概要

Anthropic 於 2026 年 7 月 24 日透過 VentureBeat 報告發布 Claude Opus 5 (API ID: claude-opus-5)，定位為編碼、代理任務與知識工作的日常旗艦模型，亦為 Claude Max 的預設模型。定價為每百萬輸入 token 5 美元、每百萬輸出 token 25 美元（與 Opus 4.8 相同），為 Fable 5 價格的一半，同時提供 Fast mode（10/50 美元）約 2.5 倍速度。在 Frontier-Bench v0.1 與 GDPval-AA 評估中創下新 SOTA，Frontier-Bench 得分 43.3%（領先 Fable 5 的 33.7%），在 CursorBench 3.2 與 OSWorld 2.0 等基準測試中以遠低於 Fable 5 的成本達到接近或超越其表現。

## 核心價值

Claude Opus 5 證明 Anthropic 能以半成本提供接近最強模型 Fable 5 的前沿智能，使代理工作流與高頻知識任務在成本效益上實現質的飛躍。

## 應用情境與實務影響

開發者與企業現在可以較低成本部署強大的編碼與代理系統：Opus 5 在 CursorBench 3.2 上僅需 Fable 5 一半成本即可達到 0.5% 差距的峰值分數；在 OSWorld 2.0 電腦使用基準上，僅需三分之一成本即可超越 Fable 5 的最佳結果。此定價策略降低了大規模 AI 代理部署的門檻。

## 補充細節

同步發布的技術部落格與基準解析顯示，Opus 5 在多項基準上 outright 超越 Fable 5（如 GDPval-AA），同時保持與 Opus 4.8 相同的努力控制機制，允許用戶根據需求在智能與速度/成本間平衡。模型支援 1M-token 上下文視窗與 128K 最大輸出，並可透過 Claude.ai、Claude Code、Anthropic API、Amazon Bedrock 與 Google Vertex AI 存取。VentureBeat 報導指出，此模型在 Anthropic 內部化學基準上比 Opus 4.8 高 10.2 個百分點，顯示其在科學研究領域的實用價值。

## 維護紀錄

- 收錄日期：2026-10-07
- 最後更新：2026-10-07

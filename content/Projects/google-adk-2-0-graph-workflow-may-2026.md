---
title: "Google 發布 Agent Development Kit (ADK) 2.0：圖基工作流執行引擎與多代理協作正式版"
type: project
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-05-19"
organization: "Google"
source_url: "https://developers.googleblog.com/why-we-built-adk-20"
date_collected: "2026-08-25"
date_updated: "2026-08-25"
tags:
  - ai
  - project
---

# Google 發布 Agent Development Kit (ADK) 2.0：圖基工作流執行引擎與多代理協作正式版

## 基本資訊

- 發布日期：2026-05-19
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://developers.googleblog.com/why-we-built-adk-20

## 概要

Google 於 2026 年 5 月 19 日釋出 ADK Python 2.0 GA，6 月 30 日釋出 ADK Go 2.0 GA。核心架構從階層式代理執行器重構為圖基工作流執行引擎，支援確定性執行路徑、人工審核閘、動態工作流適應與協作式多代理系統。提供 CLI 開發部署流程、多模型支援（Gemini、Claude、Ollama 等）與 Google Cloud 託管部署。

## 核心價值

以圖基執行引擎取代階層式架構，將代理、工具、函式視為工作流圖節點，實現生產級確定性、可觀測性與人工介入控制。

## 應用情境與實務影響

開發者可在本地以 CLI 從開發到部署 30 分鐘內完成；企業獲得原生多模型、多雲、可審計的代理開發框架；A2A 協定支援跨框架代理互操作。

## 補充細節

官方部落格由 Swapnil Agarwal、Alan Blount、Frank Guan 撰寫，發布於 2026-07-01，回顧 5/19 Python GA 歷程。關鍵變更：(1) Workflow Runtime 以圖節點評估代理/工具/函式；(2) 事件 Schema 與自定義會話儲存重設計；(3) 模組匯入路徑變更；(4) Go 版 2.1.0 於 6/30 GA 引入 agent.Context 統一工具上下文。2/27 宣布 ADK 工具與整合生態系統（GitHub、Jira、MongoDB、OpenTelemetry/MLflow）。同期競品：Microsoft Agent Framework 1.0 (4/3)、LangGraph 1.0 (2025-10)、Pydantic AI V2 (6/2026)、Amazon Bedrock AgentCore (6/2026)。

## 維護紀錄

- 收錄日期：2026-08-25
- 最後更新：2026-08-25

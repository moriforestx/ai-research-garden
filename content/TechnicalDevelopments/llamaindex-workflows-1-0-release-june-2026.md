---
title: "LlamaIndex Workflows 1.0 正式發布"
type: technical-development
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-06-30"
organization: "LlamaIndex"
source_url: "https://deepakbagada.in/journal/llamaindex-workflows-1-0-event-driven-engine-2026"
date_collected: "2026-08-29"
date_updated: "2026-08-29"
tags:
  - ai
  - technical-development
---

# LlamaIndex Workflows 1.0 正式發布

## 基本資訊

- 發布日期：2026-06-30
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://deepakbagada.in/journal/llamaindex-workflows-1-0-event-driven-engine-2026

## 概要

LlamaIndex 於 2026 年 6 月 30 日正式發布 Workflows 1.0 作為獨立的事件驅動框架，用於建構多步驟代理人系統。提供 Python 和 TypeScript 版本，具有型別事件處理器、共享上下文和控制流，無需 llama-index 依賴，支援資源註入和選擇性 OpenTelemetry 整合。

## 核心價值

獨立套件與事件驅動架構，提供更細緻的控制和更好的模組化

## 應用情境與實務影響

適用於需要複雜多步驟推理、工具使用和狀態管理的 AI 代理人應用

## 補充細節

框架包含 `llamaindex-workflows` Python 套件和 `@llamaindex/workflow-core` TypeScript 套件。支援 `@step` 方法進行事件處理，內建事件收集機制 (`ctx.collect_events`)，並可透過 `ctx.send_event` 發送自訂事件。已整合 LlamaCloud (parsers + indexes) 以支援 RAG-heavy 代理人，並提供視覺化工具除錯工作流程。

## 維護紀錄

- 收錄日期：2026-08-29
- 最後更新：2026-08-29

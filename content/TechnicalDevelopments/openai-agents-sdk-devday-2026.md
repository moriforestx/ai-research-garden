---
title: "OpenAI 於 DevDay 2026 發布 Agents SDK 與 Dots：Responses API 整合網路搜尋、檔案搜尋與電腦使用工具，打造企業級多代理平台"
type: technical-development
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-09-29"
organization: "OpenAI"
source_url: "https://openai.com/index/devday-2026"
date_collected: "2026-10-07"
date_updated: "2026-10-07"
tags:
  - ai
  - technical-development
---

# OpenAI 於 DevDay 2026 發布 Agents SDK 與 Dots：Responses API 整合網路搜尋、檔案搜尋與電腦使用工具，打造企業級多代理平台

## 基本資訊

- 發布日期：2026-09-29
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://openai.com/index/devday-2026

## 概要

OpenAI 於 2026 年 9 月 29 日 DevDay 大會發布一系列代理（Agent）相關更新：核心包括 Responses API（結合 Chat Completions 簡潔性與 Assistants API 工具使用能力）、內建工具（網路搜尋、檔案搜尋、電腦使用）、Agents SDK（開源協調框架，支援多代理工作流與可觀測性）以及 Dots（一直開啟的 AI 代理）。電腦使用工具由 CUA 模型驅動，在 OSWorld 基準上達成 38.1% 全場景成功率；Agents SDK 提供內建可觀測性工具用於效能分析與除錯。此發布標誌著 OpenAI 從實驗性 Swarm 框架過渡至企業級多代理堆疊，Assistants API 將於 2026 年 8 月 26 日停止服務，Responses API 與 Agents SDK 成為新預設。

## 核心價值

首次將網路搜尋、檔案檢索與電腦自動化三種能力統一於單一 API primitive 中，配合開源 SDK 的協調功能，使開發者能構建從簡單聊天機器人至複雜多代理自動化工作流的完整代理應用。

## 應用情境與實務影響

企業現在可使用 OpenAI 官方堆疊建立生產就緒的代理系統：客服代理可即時搜尋產品文檔並執行退款流程；研究代理可自動進行文獻閱讀、資料分析與報告撰寫；開發代理則能編寫、測試與部署程式碼。內建 tracing 與 observability 降低了多代理系統的除錯複雜度，而 Dots 提供持續運作的後台代理能力。

## 補充細節

根據 DevDay 2026 主題演講與技術分享，電腦使用工具在 WebArena 上達成 58.1% 成功率，在 WebVoyager 上達到 87%；Agents SDK 支援自訂工具整合、MCP 連接器與 Guardrails 安全庫；Dots 代理可作為永久服務運行，透過事件觸發或排程執行背景任務。GitHub 倉庫 @openai/openai-agents-python 已於 9 月 29 日同步公開，支援 Python ≥ 2.25.0。

## 維護紀錄

- 收錄日期：2026-10-07
- 最後更新：2026-10-07

---
title: "Microsoft 發布 Agent Framework 1.0：統一 AutoGen 與 Semantic Kernel，推出 Agent Harness 與 CodeAct"
type: technical-development
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-06-03"
organization: "Microsoft"
source_url: "https://devblogs.microsoft.com/agent-framework/microsoft-agent-framework-at-build-2026-announce"
date_collected: "2026-07-25"
date_updated: "2026-07-25"
tags:
  - ai
  - technical-development
---

# Microsoft 發布 Agent Framework 1.0：統一 AutoGen 與 Semantic Kernel，推出 Agent Harness 與 CodeAct

## 基本資訊

- 發布日期：2026-06-03
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://devblogs.microsoft.com/agent-framework/microsoft-agent-framework-at-build-2026-announce

## 概要

Microsoft 於 2026 年 4 月 2 日正式發布 Microsoft Agent Framework (MAF) 1.0 GA 版，統一 AutoGen 與 Semantic Kernel 為單一支援平台。於 BUILD 2026 發表三項重大更新：1) Agent Harness 整合生產模式（檔案記憶體、Shell 執行、工具核准、多模式提供者）；2) Foundry Hosted Agents 提供零縮放、VM 隔離、OpenTelemetry 觀測性；3) CodeAct 透過單一程式執行工具鏈，將工具鏈延遲降低 52.4%、token 使用降低 63.9%。支援 .NET 與 Python，提供 GitHub Copilot SDK 整合與 Handoff 多代理協作模式。

## 核心價值

統一雙代理框架為企業級平台，透過 Hosted Agents 與 CodeAct 大幅降低生產環境部署與運行成本。

## 應用情境與實務影響

開發者可透過單一 SDK 建構跨語言的生產級多代理系統，支援即時部署、可觀測性與人工回圈。GitHub、微軟內部團隊已採用 MAF 建構企業級代理應用。

## 補充細節

版本 1.0 GA 自 2026-04-02 起提供。Agent Harness 包含 FileMemoryProvider、FileAccessProvider、TodoProvider、AgentModeProvider、AgentSkillsProvider、BackgroundAgentsProvider、網路搜尋、Shell 執行（.NET）。CodeAct 在多步驟工具鏈基準測試中將時間從 27.81s 降至 13.23s，tokens 從 6,890 降至 2,489。支援 Handoff 模式實現代理間控制權轉移。

## 維護紀錄

- 收錄日期：2026-07-25
- 最後更新：2026-07-25

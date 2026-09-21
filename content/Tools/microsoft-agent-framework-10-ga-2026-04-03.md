---
title: "Microsoft Agent Framework 1.0 GA：統一 AutoGen 與 Semantic Kernel 的企業級代理框架"
type: tool
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-04-03"
organization: "Microsoft"
source_url: "https://devblogs.microsoft.com/agent-framework/microsoft-agent-framework-version-1-0"
date_collected: "2026-09-22"
date_updated: "2026-09-22"
tags:
  - ai
  - tool
---

# Microsoft Agent Framework 1.0 GA：統一 AutoGen 與 Semantic Kernel 的企業級代理框架

## 基本資訊

- 發布日期：2026-04-03
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://devblogs.microsoft.com/agent-framework/microsoft-agent-framework-version-1-0

## 概要

Microsoft 於 2026 年 4 月 3 日宣布 Microsoft Agent Framework (MAF) 1.0 同時釋出 .NET 與 Python 版本，達成 GA。MAF 統一 AutoGen (多代理編排) 與 Semantic Kernel (企業級 SDK)，提供原生 MCP (GA) 與 A2A (Beta) 協定支援、聲明式 YAML 代理配置、內建程式碼執行環境、記憶銀行會話管理、多供應商模型支援、跨執行時互通。採 MIT 授權，承諾長期支援 (LTS)，並提供從 AutoGen/Semantic Kernel 遷移指引。

## 核心價值

微軟將兩大代理專案合併為單一生產級框架，原生雙協定 (MCP+A2A) 打通跨框架代理互通，.NET/Python 同步 GA 降低企業採用門檻，LTS 承諾解決生產環境穩定性顧慮。

## 應用情境與實務影響

企業可採單一框架涵蓋從單一助手到車隊級多代理編排；原生 MCP 直通工具生態、A2A 未來實現跨框架協作；遷移工具保護既有投資；Azure AI Foundry 整合提供託管運行選項。

## 補充細節

編排模式：群聊、移交、圖型工作流 (含檢查點與時光旅行除錯)。Magentic-One 管理驅動任務帳本。內建代碼執行環境減少樣板代碼。範例涵蓋多供應商、Ollama/ONNX 本地模型、工作流。GitHub: microsoft/agent-framework。InfoQ 報告 2026-06 Build 進一步釋出 Agent Harness 與 Foundry Hosted Agents GA。

## 維護紀錄

- 收錄日期：2026-09-22
- 最後更新：2026-09-22

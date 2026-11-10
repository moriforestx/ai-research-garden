---
title: "LangChain 發布 LangGraph 0.3：預建代理生態系統正式啟動"
type: tool
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-10-10"
organization: "LangChain"
source_url: "https://blog.langchain.com/langgraph-0-3-release-prebuilt-agents"
date_collected: "2026-11-11"
date_updated: "2026-11-11"
tags:
  - ai
  - tool
---

# LangChain 發布 LangGraph 0.3：預建代理生態系統正式啟動

## 基本資訊

- 發布日期：2026-10-10
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://blog.langchain.com/langgraph-0-3-release-prebuilt-agents

## 概要

LangChain 於 2026 年 10 月發布 LangGraph 0.3，將 `create_react_agent` 拆出至獨立 `langgraph-prebuilt` 套件，並推出預建代理生態系統：Trustcall（結構化擷取）、LangGraph Supervisor（Supervisor 多代理架構）、LangMem（長期記憶）、LangGraph Swarm（Swarm 多代理架構）。支援 Python 與 JavaScript，提供建立自訂預建代理的指南與註冊機制。

## 核心價值

以預建代理模組化降低多代理系統開發門檻，建立可擴展的社群生態系統（參照 LangChain 700+ 整合模式）。

## 應用情境與實務影響

開發者可直接使用生產級預建代理快速構建 Supervisor、Swarm、長期記憶等常見架構；原始碼基於 LangGraph 便於客製化與除錯。

## 補充細節

發布週同步釋出相關教學：ScaleDown 與 Deep Agents 長期運行代理（10/13）、AI Search 搜尋代理追蹤（10/13）、代理評估常見問題（10/15）。預建代理採用 OCI 風格封裝，支援註冊表發佈與版本管理。

## 維護紀錄

- 收錄日期：2026-11-11
- 最後更新：2026-11-11

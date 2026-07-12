---
type: tool
name: "Agent Skills"
score: "4"
date_collected: "2026-07-12"
source_url: "https://github.com/addyosmani/agent-skills"
tags:
  - ai
  - tool
  - agent-framework
  - open-standard
---

# Agent Skills

## 這是什麼

由 Google Chrome 團隊工程師 Addy Osmani 主導的開源專案，定義 AI Agent 技能的開放標準規格。提供標準化的技能描述格式、註冊表、發現機制和執行運行時，讓不同框架、不同廠商的 Agent 能夠共享、組合和復用技能。

## 主要功能

- 統一的技能描述 Schema（JSON Schema），包含名稱、描述、參數、返回值、前置條件、副作用等元數據
- 技能註冊表協議，支援分佈式技能發現和版本管理
- 參考實現：TypeScript/JavaScript 運行時，支援技能動態載入、參數驗證、執行追蹤
- 內建常用技能庫：Web 搜尋、代碼執行、文件操作、API 調用、瀏覽器自動化等
- 與 LangChain、AutoGen、CrewAI、OpenAI Agents SDK 等主流框架的適配器

## 為什麼重要

解決 AI Agent 生態碎片化的核心問題：
- 技能不可跨框架復用：LangChain 的 Tool 無法直接在 AutoGen 中使用
- 缺乏標準發現機制：無法像 npm/pip 一樣搜尋、安裝、更新 Agent 技能
- 版本衝突和相容性問題：技能接口變更導致 Agent 失效
- 重複造輪子：每個團隊都在重寫相同的基礎技能（搜尋、代碼執行、文件讀寫）

## 可能影響

- 建立「Agent 技能經濟」：技能開發者可發布、分發、甚至商業化技能
- 降低多 Agent 系統開發門檻：像搭積木一樣組裝複雜 Agent 工作流
- 推動企業級 Agent 治理：統一的技能審計、權限控制、合規檢查介面
- 影響 OpenAI、Anthropic、Google、Microsoft 等大廠的 Agent 平台策略

## 相關概念

- [[Multi-Agent Orchestration]]
- [[Agent Framework Selection]]
- [[OpenAI Agents SDK]]
- [[LangGraph]]
- [[AutoGen]]
- [[MCP Server]]

## 更新紀錄

- 2026-07-12：首次收錄（GitHub Trending 當日星標 1,116+）。

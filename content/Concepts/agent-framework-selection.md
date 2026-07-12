---
type: concept
name: "Agent Framework Selection"
date_updated: "2026-07-12"
tags:
  - concept
  - ai-agent
  - framework
  - selection
---

# Agent Framework Selection

## 定義

根據專案複雜度、團隊專長、生產要求、廠商鎖定風險等維度，在 LangGraph、CrewAI、AutoGen、OpenAI Agents SDK、Microsoft Semantic Kernel、Google ADK 等主流 Agent 框架中進行技術選型的決策方法論。核心考量：狀態管理模式（圖 vs 角色 vs 對話）、部署目標（雲端 vs 本地 vs 混合）、可觀測性內建程度、生態系統成熟度、長期維護承諾。

## 為什麼重要

- 避免「為了用框架而用框架」的過度設計，簡單工作流不需要多 Agent 編排
- 降低技術債務：框架選型錯誤導致的重構成本極高（狀態管理、記憶、工具調用全部耦合）
- 廠商鎖定風險：OpenAI Agents SDK 強綁定 OpenAI 生態，AutoGen 綁定 Microsoft，LangGraph 相對中立

## 出現在哪些內容

- [[AI Agent Orchestration Multi-Agent Workflow Guide]]
- [[Daily/2026-07-12]]

## 相關概念

- [[Multi-Agent Orchestration]]
- [[LangGraph]]
- [[CrewAI]]
- [[AutoGen]]
- [[OpenAI Agents SDK]]
- [[Vendor Lock-in]]
- [[Agent Maturity Model]]

## 更新紀錄

- 2026-07-12：首次建立。

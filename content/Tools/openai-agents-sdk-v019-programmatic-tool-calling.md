---
title: "OpenAI Agents SDK v0.19.0 釋出：新增程式化工具呼叫，強化代理開發能力"
type: tool
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-07-27"
organization: "OpenAI"
source_url: "https://github.com/openai/openai-agents-python/releases/tag/v0.19.0"
date_collected: "2026-07-29"
date_updated: "2026-07-29"
tags:
  - ai
  - tool
---

# OpenAI Agents SDK v0.19.0 釋出：新增程式化工具呼叫，強化代理開發能力

## 基本資訊

- 發布日期：2026-07-27
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://github.com/openai/openai-agents-python/releases/tag/v0.19.0

## 概要

OpenAI 於 2026 年 7 月 27 日發布 Agents Python SDK v0.19.0，此版本雖不包含破壞性變更，但因應 OpenAI Responses API 新增「程式化工具呼叫」功能而升級次版本號。開發者現在可透過程式碼直接定義、組合與調度工具，而非僅依賴模型自行決定工具調用時機，大幅提升代理工作流的可控性與可觀測性。

## 核心價值

將工具呼叫從模型隱式決策轉為開發者顯式編程控制，降低生產環境中代理行為不可預測的風險。

## 應用情境與實務影響

支援複雜多步驟代理管線（如：檢查檔案 → 依條件呼叫不同工具 → 聚合結果）、除錯時可精確重現工具調用序列、易於加入自訂前後處理邏輯。SDK 繼續保持輕量設計，適合快速原型與生產部署。

## 補充細節

v0.19.0 對應 GitHub 提交 a2d8270，由 @seratch 簽署發布。更新內容包含：依賴升級、動作版本更新、文件微調、測試覆蓋率提升（_openai_retry helpers 從 77% 達 95%）、新增 run_demo_loop 串流與空輸入路徑單元測試。完整變更日誌見 GitHub Releases 頁面。此版本需搭配支援 Programmatic Tool Calling 的 OpenAI Responses API 使用。

## 維護紀錄

- 收錄日期：2026-07-29
- 最後更新：2026-07-29

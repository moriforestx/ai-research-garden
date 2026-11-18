---
title: "LangChain 發布 Managed Deep Agents v0.10：瀏覽器操作與非同步子代理正式上線"
type: tool
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-10-29"
organization: "LangChain"
source_url: "https://www.langchain.com/blog/managed-deep-agents-browser-use-and-asynchronous-subagents"
date_collected: "2026-11-19"
date_updated: "2026-11-19"
tags:
  - ai
  - tool
---

# LangChain 發布 Managed Deep Agents v0.10：瀏覽器操作與非同步子代理正式上線

## 基本資訊

- 發布日期：2026-10-29
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://www.langchain.com/blog/managed-deep-agents-browser-use-and-asynchronous-subagents

## 概要

LangChain 於 2026-10-29 釋出 Managed Deep Agents v0.10 (公測自 8/7 起)，新增兩大核心能力：(1) 瀏覽器操作 —— 內建四種瀏覽器工具，支援無 API 網站自動化，登入時可將視窗移交人工處理，密碼不進模型上下文；(2) 非同步子代理 —— 子代理可在背景執行緒長時間運行，不阻塞主對話，提供啟動、查詢、更新、取消工具與完成通知機制。同步釋出執行緒來源追蹤 (Slack 回覆歸屬) 與停止鈕取消執行。Python/JS SDK 僅需在 subagent 定義加 `async: True` 即可啟用。

## 核心價值

將「瀏覽器自動化」與「非同步任務編排」納入代理運行時標準庫，解決長任務阻塞對話、憑證隔離等生產痛點，推動代理從示範走向可交付服務。

## 應用情境與實務影響

開發者可直接部署會預訂機票、填表單、後台跑報表的代理，無需自建瀏覽器基礎設施；非同步模式讓使用者體驗從「等待回應」轉為「持續對話、稍後收結果」。

## 補充細節

官方部落格 2026-10-29 發文，X 貼文同步宣傳、LinkedIn 專業社群轉發；v0.10 版本號、發布日期、功能清單、代碼範例、公測時間線 (8/7 起) 均可驗證。

## 維護紀錄

- 收錄日期：2026-11-19
- 最後更新：2026-11-19

---
title: "Model Context Protocol Draft Specification Updates — June 2026"
type: technical-development
research_topic: "AI 代理人 / AI Agents"
date_published: "2026-06-12"
date_collected: "2026-07-14"
date_updated: "2026-07-14"
source_url: "https://github.com/modelcontextprotocol/specification"
identifier: "model-context-protocol-draft-2026-06"
tags:
  - ai
  - technical-development
  - ai-agents
  - mcp
  - protocol
  - specification
  - tool-integration
---

# Model Context Protocol Draft Specification Updates — June 2026

## 概述

Model Context Protocol（MCP）官方規範 Repository 在 2026 年 6 月持續更新 draft specification。此次收錄聚焦 6 月 7 日至 12 日間的實質規範變更，而不是將其描述為新的正式穩定版本。

截至本次收錄，Repository 中最新的穩定版本目錄仍為 `2025-11-25`；2026 年的內容主要位於 `draft`。

## 本次主要變更

近期 draft 規範更新包含：

- 定義 JSON-RPC 錯誤碼配置政策
- 調整 draft 使用的錯誤碼範圍
- 重新定義 subscription ID 的格式與傳遞方式
- 明確訂閱、取消與回應順序
- 對完整結果的快取要求與 cache key 進行規範
- 移除或調整 SSE resumability 相關要求
- 同步 draft schema 與規範文件
- 改善 discover response 的資料型別說明

## 技術意義

這些變更反映 MCP 正逐步處理協議實作時容易產生不一致的細節，例如錯誤碼衝突、訂閱識別、串流恢復、快取邊界與 schema 對齊。

對開發 MCP client、server 或代理人工具整合平台的團隊而言，這些規範細節會直接影響：

- client 與 server 的互通性
- 錯誤處理一致性
- 長連線與訂閱管理
- 結果快取與重試邏輯
- draft 與未來穩定版本的相容性

## 應用情境與實務影響

- AI 代理人工具介面標準化
- MCP client 與 server 實作
- IDE、代理平台與外部工具整合
- 權限與錯誤處理機制設計
- 串流、訂閱與長時間任務管理
- 協議相容性測試

## 使用與部署注意事項

- 目前收錄的是 draft specification，不是新的正式穩定版本。
- draft 內容仍可能在正式版本前更動。
- 生產環境應明確鎖定支援的 MCP specification version。
- 不應僅追蹤 Repository 最新 commit，需區分文件修正、相依套件更新與實質協議變更。
- client 與 server 應建立版本協商及相容性測試。

## 限制與待觀察事項

- 2026 年尚未出現新的穩定版本目錄。
- `2026-07-28-RC` 對本次收錄日期而言仍是未來候選版本，不能視為已發布版本。
- draft 變更可能在正式 release 前再次調整。

## 來源

- 官方規範 Repository：https://github.com/modelcontextprotocol/specification
- Draft specification：https://github.com/modelcontextprotocol/specification/tree/main/docs/specification/draft
- 本次收錄基準日期：2026-06-12

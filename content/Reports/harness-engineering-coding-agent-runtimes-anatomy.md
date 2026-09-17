---
title: "Harness Engineering：十一套生產級編程代理運行時的源碼解剖與架構演進"
type: report
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-02"
organization: "Multiple institutions"
source_url: "https://arxiv.org/abs/2609.00006"
date_collected: "2026-09-17"
date_updated: "2026-09-17"
tags:
  - ai
  - report
---

# Harness Engineering：十一套生產級編程代理運行時的源碼解剖與架構演進

## 基本資訊

- 發布日期：2026-09-02
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.00006

## 概要

首份針對生產級編程代理運行時的大規模源碼實證研究，分析十一套主流 harness（Claude Code、Codex CLI、Gemini CLI、Mistral Vibe、OpenHands、Aider、Mini-SWE-Agent、Hermes、Pi、OpenCode、OpenClaw）及首個元 harness Omnigent。定義 harness 七大標準子系統（循環、工具、上下文管理、安全控制、編排、擴展介面、狀態持久化），�出 13 項跨系統觀察與 29 個週期性設計模式。關鍵發現：無系統引入通用代理框架、無系統採用向量嵌入檢索、skills 採用率超過 MCP (9/11 vs 8/11)、ACP 已在 6 系統部署並引入「harness 托管」新角色。縱向對比顯示：harness 在 2026 上半年完成從工具到平台的轉型，行為策略從提示詞散文遷移至配置化。附 18 項設計建議與 90 行最小可行 harness 脚手架。

## 核心價值

為 harness engineering 確立實證基礎，揭示代理部署運行時的演化軌跡與共性模式，指導生產級 AI 代理系統的架構決策。

## 應用情境與實務影響

開發者可依據 29 設計模式與 18 建議構建/選型 harness；研究者獲得受控縱向樣本追蹤領域演化；企業可評估代理部署成熟度與風險。

## 補充細節

論文於 2026-07-15 提交 (v1)，2026-09-02 發布。涵蓋約 400 萬行 Python/TypeScript/Rust 代碼。作者：Paul Barbaste 等。主體：Software Engineering (cs.SE)、Multiagent Systems (cs.MA)。包含 OpenClaw 在內的十一套系統源碼級解剖。

## 維護紀錄

- 收錄日期：2026-09-17
- 最後更新：2026-09-17

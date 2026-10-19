---
title: "Meta releases open-weight Muse Spark model for coding, agentic tasks"
type: tool
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-10-15"
organization: "Meta AI"
source_url: "https://www.reuters.com/business/meta-releases-open-weight-muse-spark-model-coding-agentic-tasks-2026-10-15"
date_collected: "2026-10-20"
date_updated: "2026-10-20"
tags:
  - ai
  - tool
---

# Meta releases open-weight Muse Spark model for coding, agentic tasks

## 基本資訊

- 發布日期：2026-10-15
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://www.reuters.com/business/meta-releases-open-weight-muse-spark-model-coding-agentic-tasks-2026-10-15

## 概要

Meta 於 2026-10-15 發布 Muse Spark Open，為開放權重的多模態稀疏混合專家模型 (MoE)，總參數約 816B、啟動參數約 42B、支援高達 1M tokens 上下文。原生支援文本、圖像、音訊、視頻輸入，針對編碼與代理任務優化（多檔案重構、長除錯會話、網頁瀏覽規劃/執行/觀察/自我修正）。採用 Harmony 聊天模板，權重託管於 Hugging Face，可於 Together、Fireworks、Groq 等平台部署。授權為 Meta Muse Model License (非開源，需歸屬、超過 2000 萬美元營收需額外協議)。

## 核心價值

首個前沿級開放權重多模態 MoE 模型專為代理工作流設計，提供 1M 上下文與 42B 活躍參數的高效推理，大幅降低自建代理系統門檻。

## 應用情境與實務影響

開發者可下載權重自行部署或使用託管 API，構建具備多模態感知、長程規劃、工具使用、自我修正能力的代理應用；MCP Atlas 基準達 89.2%，證明代理任務強項。雙 M5 Ultra Mac Studio 即可運行，硬體門檻相對可控。

## 補充細節

Reuters 報導確認 2026-10-15 發布。Hugging Face 部落格 (https://huggingface.co/blog/meta-muse-spark-open) 提供技術細節：256 專家/層、每 token 路由 8 專家、BF16 檢查點約 1.5 TB。AI Release Tracker 記錄同期發布 Muse Wonder (10/12) 與 Muse Wonder Full (10/12)。授權條款：Muse Model License，要求歸屬，商業化門檻 2000 萬美元。

## 維護紀錄

- 收錄日期：2026-10-20
- 最後更新：2026-10-20

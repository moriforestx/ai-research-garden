---
title: "Anthropic 發布 Claude Fable 5.1 與 Mythos 5.1"
type: tool
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-09-01"
organization: "Anthropic"
source_url: "https://www.anthropic.com/news/claude-fable-5-1-mythos-5-1"
date_collected: "2026-09-07"
date_updated: "2026-09-07"
tags:
  - ai
  - tool
---

# Anthropic 發布 Claude Fable 5.1 與 Mythos 5.1

## 基本資訊

- 發布日期：2026-09-01
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://www.anthropic.com/news/claude-fable-5-1-mythos-5-1

## 概要

Anthropic 於 2026 年 9 月 1 日正式發布 Claude Fable 5.1 及其可信存取對應版本 Mythos 5.1。Fable 5.1 為 Fable 5 的同權重刷新版，保持 1M token 上下文窗口與 128K 最大輸出，但快取讀取價格從 $1.00 降至 $0.25 每百萬 token（降幅 75%），官方估算典型工作負載成本降約 25%，高度代理任務最高可降 45%。Mythos 5.1 為相同模型權重但移除安全防護，僅透過 Fairwind 計畫提供給經審核的防禦研究者。兩模型同步上線 Claude、Claude Code、Claude Platform 與 Cursor。

## 核心價值

重大成本降低（快取讀取 -75%）與雙軌發布策略（通用版 + 防禦研究版），展示前沿實驗室在經濟效率與安全治理上的並行創新。

## 應用情境與實務影響

開發者與企業可大幅降低長對話、代理迴圈等高快取命中場景的推理成本；安全研究社群獲得可控環境測試模型極限能力的官方管道。

## 補充細節

發布同步包含三項破壞性 API 變更：cache-read 價格調整、工具呼叫格式微調、回應結構標準化。Anthropic 官方部落格與開發者文件均於 9 月 1 日上線，X 官方帳號 @claudeai 同步宣傳。

## 維護紀錄

- 收錄日期：2026-09-07
- 最後更新：2026-09-07

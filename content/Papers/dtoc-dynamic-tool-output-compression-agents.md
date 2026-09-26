---
title: "DTOC: Dynamic Tool Output Compression for Adaptive Context Management in AI Agents"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-08-06"
organization: "Pegasystems / Leiden University"
source_url: "https://arxiv.org/abs/2609.26121"
date_collected: "2026-09-27"
date_updated: "2026-09-27"
tags:
  - ai
  - paper
---

# DTOC: Dynamic Tool Output Compression for Adaptive Context Management in AI Agents

## 基本資訊

- 發布日期：2026-08-06
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2609.26121

## 概要

Pegasystems 與 Leiden University 研究團隊提出 DTOC（動態工具輸出壓縮），解決長視野 AI 代理人的核心瓶頸：有限上下文窗口導致的「上下文腐爛」。DTOC 將上下文管理重構為代理人可顯式控制的可逆操作：完整工具輸出儲存於外部記憶體，活躍上下文僅保留輕量佔位符（tool_key、時間戳、token 估算），代理人透過 `manage_context` 工具動態啟用/停用輸出。關鍵創新：(1) 非破壞性壓縮，保留完整可恢復性；(2) 代理人主導的自適應壓縮策略，而非固定啟發式；(3) 模型無關的統一介面。DeepSWE 基準測試顯示：對響應模型 (Sonnet 4.6, GPT-5.4)，DTOC 減少輸入 token 10-13%、代理步數 2-32%，解題率提升 1.5-2.5 倍，單解題成本降低 3-3.5 倍；消融實驗證明可逆性關鍵——僅停用版本效能下降，完整 DTOC 以大幅更低上下文成本恢復基準準確率。已獲 Discovery Science 2026 (10/5-10/9, Mainz) 接受。開源實作：https://github.com/chaturvediabhay24/opencode

## 核心價值

將上下文管理從系統級啟發式提升為代理人級顯式推理動作，為長視野代理系統（程式編輯、科學研究、自主規劃）提供可生產部署的可逆壓縮範式。

## 應用情境與實務影響

直接降低企業級代理部署的 token 成本與延遲；解決 Gartner 預測的 50% 代理部署因上下文治理不足而失敗的問題；支援 OpenCode、OpenHands、Cursor 等主流代理框架整合。

## 補充細節

arXiv:2609.26121v1 [cs.AI]，提交日期 2026-08-06。作者：Abhay Chaturvedi、Shreya Bhattacharya、Rashmika Gopalkrishnan (Pegasystems Bangalore)、Peter van der Putten (Pegasystems Amsterdam / LIACS Leiden Univ.)。接受 Discovery Science 2026 (2026-10-05 至 10-09, Mainz, Germany)。License: CC BY-NC-ND 4.0。屬 AI Agents 核心架構與上下文工程研究。

## 維護紀錄

- 收錄日期：2026-09-27
- 最後更新：2026-09-27

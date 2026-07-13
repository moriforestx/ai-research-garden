---
title: "SafeSeek: Universal Attribution of Safety Circuits in Language Models"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-07-01"
authors:
  - "Qingsong Wen Research Team"
keywords:
  - "safety circuits"
  - "mechanistic interpretability"
  - "language model safety"
  - "ICML 2026"
  - "attribution methods"
identifier: "ICML2026-SafeSeek"
identifier_type: "conference"
publication_status: "published"
source_url: "https://icml.cc/virtual/2026/poster/XXXXX"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# SafeSeek: Universal Attribution of Safety Circuits in Language Models

## 基本資訊

- 作者：Qingsong Wen 研究團隊
- 發布日期：2026-07-01 (ICML 2026)
- 研究主題：AI 代理人 / AI Agents
- 關鍵字：safety circuits、mechanistic interpretability、language model safety、ICML 2026、attribution methods
- 論文識別碼：ICML2026-SafeSeek (conference)
- 發表狀態：已發表
- 主要來源：https://icml.cc/virtual/2026/poster/XXXXX

## 摘要

提出 SafeSeek，一種通用的安全電路歸因方法，能在語言模型中識別並定位負責安全行為的神經電路。透過因果介入與反事實分析，揭示模型如何在不同安全情境下激活特定計算路徑。

## 核心研究問題

如何系統性地識別並歸因語言模型內部負責安全決策的計算電路？

## 方法與技術

1. **電路發現**：基於激活修補與路徑修補技術，追蹤安全相關 Token 的資訊流
2. **普適歸因框架**：跨模型、跨任務的安全電路識別演算法
3. **因果驗證**：透過干預實驗確認電路對安全行為的必要性與充分性

## 實驗與研究結果

在多個開源模型 (Llama, Qwen, Gemma 等) 與安全基準上驗證，發現存在共享的安全電路結構，且可透過微調選性增強或抑制特定安全行為。

## 研究意義與適用範圍

為 AI 代理人安全提供機制級解釋工具，支援安全對齊驗證、紅隊測試與可解釋安全機制設計。

## 限制與注意事項

電路識別需白盒存取模型權重；閉源模型無法直接應用；計算成本較高。

## 相關概念

- 機制解釋性
- 安全對齊
- 因果介入
- AI 代理人安全

## 相關工具與專案

- ICML 2026 論文頁面

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

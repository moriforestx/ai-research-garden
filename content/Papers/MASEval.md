---
title: "MASEval: Extending Multi-Agent Evaluation from Models to Systems"
type: paper
research_topic: "AI 代理人 / AI Agents"
date_published: "2026-03-09"
date_collected: "2026-07-15"
date_updated: "2026-07-15"
source_url: "https://arxiv.org/abs/2603.08835"
identifier: "arxiv-2603-08835"
tags:
  - ai
  - paper
---

# MASEval: Extending Multi-Agent Evaluation from Models to Systems

## 基本資訊

- 作者：Cornelius Emde、Alexander Rubinstein、Anmol Goel、Ahmed Heakl、Sangdoo Yun、Seong Joon Oh、Martin Gubri
- 發布日期：2026-03-09
- 研究主題：AI 代理人 / AI Agents
- 關鍵字：Multi-Agent Evaluation、Agent Framework、System-Level Evaluation、Benchmarking、ACL 2026
- 論文識別碼：arXiv:2603.08835v1
- 發表狀態：已發表 (ACL 2026 Demo Track)
- 主要來源：https://arxiv.org/abs/2603.08835

## 摘要

MASEval 提供一個統一評估層，實現跨代理框架和基準的系統級無框架比較。當前代理評估主要關注模型級能力，忽略了框架層面的設計選擇（如記憶、工具調用、規劃模組）對系統性能的影響。MASEval 將整個代理系統作為分析單元，跨 3 個基準 (GAIA, MACS, Tau2)、3 個模型、3 個框架 (AutoGen, LangGraph, smolagents) 進行首次系統級系統性比較。研究發現：在可比成本與能力的模型下，框架選擇對性能的影響與模型選擇同等重要。

## 核心研究問題

如何建立框架無關的多代理系統級評估標準，量化框架設計選擇對系統性能的影響？

## 方法與技術

1. **統一評估層**：MASEval 提供 Python 像一個薄包裝層，將任何代理系統標準化為可評估介面，不侵入框架內部。
2. **系統級分析單元**：以完整代理系統（模型+框架+配置）而非單獨模型為評估單位。
3. **跨維度系統性比較**：3 基準 × 3 模型 × 3 框架 = 27 系統配置的完整矩陣評估。
4. **模組化設計空間**：參考 AgentSquare 將代理分解為規劃、推理、工具使用、記憶四大功能模組。

## 實驗與研究結果

- **框架效應顯著**：同一模型下，不同框架性能差異可達 15-20% 絕對分數。
- **框架選擇 ≈ 模型選擇**：在可比成本/能力模型下，框架影響與模型影響同量級。
- **基準敏感性**：不同基準對框架敏感度不同，GAIA 偏向工具使用，MACS 偏向記憶規劃。
- **開源框架競爭力**：smolagents 等輕量框架在特定任務上可匹配商業框架。

## 研究意義與適用範圍

- 建立首個多代理系統級評估標準與開源工具。
- 量化證明框架設計選擇的關鍵性，指導實務選型。
- 為代理框架開發者提供標準化基準。
- 適用於代理系統選型、框架開發、學術基準建設。

## 限制與注意事項

- 僅覆蓋 3 個主流框架，新興框架 (如 OpenAI Agents SDK, Google ADK) 待補充。
- 基準主要為通用推理任務，垂直領域 (編程、科研、金融) 需專門基準。
- 評估成本較高，完整矩陣需大量計算資源。

## 相關概念

- Multi-Agent Systems
- Agent Framework
- System-Level Evaluation
- Benchmarking

## 相關工具與專案

- MASEval 官方庫：https://github.com/MASEval/MASEval (推測)
- AutoGen: https://github.com/microsoft/autogen
- LangGraph: https://github.com/langchain-ai/langgraph
- smolagents: https://github.com/huggingface/smolagents

## 維護紀錄

- 收錄日期：2026-07-15
- 最後更新：2026-07-15
- 更新紀錄：
  - 2026-07-15：首次建立

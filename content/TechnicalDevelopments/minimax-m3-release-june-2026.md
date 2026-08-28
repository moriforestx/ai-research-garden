---
title: "MiniMax M3 開放權重模型發布"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-06-01"
organization: "MiniMax"
source_url: "https://www.marktechpost.com/2026/06/01/minimax-releases-minimax-m3-with-msa-architecture-supporting-1m-token-context-native-multimodality-and-agentic-coding"
date_collected: "2026-08-29"
date_updated: "2026-08-29"
tags:
  - ai
  - technical-development
---

# MiniMax M3 開放權重模型發布

## 基本資訊

- 發布日期：2026-06-01
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://www.marktechpost.com/2026/06/01/minimax-releases-minimax-m3-with-msa-architecture-supporting-1m-token-context-native-multimodality-and-agentic-coding

## 概要

MiniMax 於 2026 年 6 月 1 日發布 MiniMax M3，這是一個開放權重的混合專家(MoE)模型，具有 428 億總參數（約 23 億活躍參數/token）、100 萬 token 上下文視窗，以及原生圖像和視訊輸入能力。採用 MiniMax Sparse Attention (MSA) 架構，在 1M token 長度下將計算需求降至前一代的約 1/20。

## 核心價值

首個結合編碼、長上下文推理和原生多模態理解的開放權重模型

## 應用情境與實務影響

適用於需要長上下文處理、編程、代理人工作流程和多模態理解的複雜 AI 應用

## 補充細節

模型在 SWE-Bench Pro 上達到 59.0% 分數，超越 GPT-5.5 和 Gemini 3.1 Pro。在 OSWorld-Verified 電腦使用基準上達 70.06%。技術報告於 2026 年 6 月 11 日發布於 arXiv，模型權重於 6 月 7 日上傳至 Hugging Face。API 於發布當天即時上線，支援 OpenAI-compatible 和 Anthropic Messages 端點。

## 維護紀錄

- 收錄日期：2026-08-29
- 最後更新：2026-08-29

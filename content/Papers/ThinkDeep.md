---
title: "Think Deep, Not Just Long: Measuring LLM Reasoning Effort via Deep-Thinking Tokens"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-06-01"
authors:
  - "ICML 2026 Authors"
keywords:
  - "reasoning effort"
  - "deep-thinking tokens"
  - "chain-of-thought"
  - "test-time scaling"
  - "ICML 2026"
identifier: "ICML2026-ThinkDeep"
identifier_type: "conference"
publication_status: "published"
source_url: "https://icml.cc/virtual/2026/poster/64256"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# Think Deep, Not Just Long: Measuring LLM Reasoning Effort via Deep-Thinking Tokens

## 基本資訊

- 作者：ICML 2026 作者群
- 發布日期：2026-06-01 (ICML 2026)
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 關鍵字：reasoning effort、deep-thinking tokens、chain-of-thought、test-time scaling、ICML 2026
- 論文識別碼：ICML2026-ThinkDeep (conference)
- 發表狀態：已發表
- 主要來源：https://icml.cc/virtual/2026/poster/64256

## 摘要

本研究挑戰「生成長度等於推理品質」的假設，提出 deep-thinking tokens 概念：在模型深層預測發生顯著修訂的 tokens。跨四大數學科學基準（AIME 24/25、HMMT 25、GPQA-diamond）與多模型（GPT-OSS、DeepSeek-R1、Qwen3）驗證，deep-thinking ratio 與準確率呈強正相關，優於長度與信心基線。據此提出 Think@n 測試時擴展策略。

## 核心研究問題

如何量化 LLM 推理過程中的真實認知努力，而非僅以生成長度為代理指標？

## 方法與技術

定義 deep-thinking tokens 為模型內部預測在深層發生顯著變化的 tokens。計算 deep-thinking ratio 作為推理努力度量。提出 Think@n 策略：優先選擇高 deep-thinking ratio 的樣本進行測試時計算擴展。

## 實驗與研究結果

在四大基準上，deep-thinking ratio 與準確率呈穩健正相關（r > 0.7），顯著優於 token 長度與信心分數。Think@n 在相同計算預算下提升準確率。

## 研究意義與適用範圍

提供可觀測的推理品質指標，指導測試時計算最佳分配，適用於數學、科學推理等高難度任務。

## 限制與注意事項

需存取模型內部層激活值；對閉源模型適用性受限。

## 相關概念

- 思維鏈
- 測試時擴展
- 推理品質評估
- 模型內部機制

## 相關工具與專案

- ICML 2026 開放獲取版本

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

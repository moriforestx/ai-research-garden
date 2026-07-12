---
title: "RAG over Thinking Traces Can Improve Reasoning Tasks"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-05-05"
authors: []
keywords: []
identifier: "2605.03344"
identifier_type: "arXiv"
publication_status: "preprint"
source_url: "https://arxiv.org/abs/2605.03344v1"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# RAG over Thinking Traces Can Improve Reasoning Tasks

## 基本資訊

- 作者：Narabzad 等人
- 發布日期：2026-05-05
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 關鍵字：檢索增強生成、思維鏈、推理任務、T3 方法
- 論文識別碼：2605.03344 (arXiv)
- 發表狀態：預印本
- 主要來源：https://arxiv.org/abs/2605.03344v1

## 摘要

本研究挑戰「RAG 對推理任務無幫助」的假設，提出將思維軌跡作為檢索語料庫，並引入 T3 方法結構化思維軌跡。實驗顯示在 AIME 基準上，Gemini-2.5-Flash 提升 56.3%、GPT-OSS-120B 提升 8.6%、GPT-5 提升 7.6%，同時推理成本降低達 15%。

## 核心研究問題

思維軌跡作為檢索語料庫是否能有效提升大型語言模型的推理能力？

## 方法與技術

提出 T3 方法：從模型生成的思維軌跡中提取關鍵推理步驟，構建結構化檢索索引，推理時檢索相關軌跡片段輔助生成。

## 實驗與研究結果

在多項數學與邏輯推理基準上顯著提升表現，並降低推理 Token 消耗。

## 研究意義與適用範圍

證明 RAG 技術可延伸至複雜推理任務，為降低大模型推理成本提供新路徑，適用於數學推理、邏輯推理等需多步思考的場景。

## 限制與注意事項

依賴模型生成高品質思維軌跡；檢索索引建構需額外計算資源。

## 相關概念

- 檢索增強生成
- 思維鏈
- 推理增強
- 結構化檢索

## 相關工具與專案

- T3 實作：https://github.com/Narabzad/t3

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

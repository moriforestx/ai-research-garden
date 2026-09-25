---
title: "MORSE: Multi-Context Ordering via Reverse Scoring for Evidence-Preserving Compression"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-09-23"
organization: "N/A (arXiv 預印本)"
source_url: "https://arxiv.org/abs/2609.27380"
date_collected: "2026-09-26"
date_updated: "2026-09-26"
tags:
  - ai
  - paper
---

# MORSE: Multi-Context Ordering via Reverse Scoring for Evidence-Preserving Compression

## 基本資訊

- 發布日期：2026-09-23
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2609.27380

## 概要

針對長上下文壓縮時證據丟失問題，提出 MORSE 方法：利用反向查詢-證據原則，對多上下文進行證據優先排序，再配合壓縮感知排列選擇，在多跳問答基準上持續優於靜態逆序與隨機搜索，有效保留關鍵支撐證據。

## 核心價值

解決上下文壓縮導致的關鍵證據遺漏，提供免訓練、即插即用的排序策略，顯著提升 RAG 與長上下文任務的可靠度。

## 應用情境與實務影響

適用於長文檔問答、多跳推理、代碼庫分析等需壓縮上下文的 LLM 應用，降低推理成本同時保持準確率。

## 補充細節

arXiv:2609.27380v1 [cs.CL]，提交日期 2026-09-23。作者：Ke Wan、Yifan Wang、Liheng Lai、Chen Chen。核心貢獻：(1) 分析靜態逆序壓縮會抑制後方強證據的增量分數；(2) 提出 MORSE 兩階段機制——個別上下文內證據優先錨點 + 壓縮候選輸出的排列選擇；(3) 在 HotpotQA、2WikiMultihopQA、MuSiQue 等基準上，跨多種壓縮方法、預算、評分模型均穩定提升證據保留率與下游 QA 表現。代碼開源。

## 維護紀錄

- 收錄日期：2026-09-26
- 最後更新：2026-09-26

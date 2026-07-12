---
type: concept
name: "RAG Optimization"
date_updated: "2026-07-12"
tags:
  - concept
  - rag
  - llm
  - optimization
---

# RAG Optimization

## 定義

針對檢索增強生成系統在檢索質量、生成質量、延遲、成本四個維度的系統性優化工程實踐。核心技術棧：查詢重寫/擴展 → 混合檢索（稀疏+稠密+圖） → 重排序 → 上下文壓縮/摘要 → 提示工程 → 生成後驗證。長文本 RAG 專項優化：分層索引、滑動窗口檢索、遞歸摘要、檢索感知微調。

## 為什麼重要

- RAG 是企業級 LLM 應用的標準架構，但朴素 RAG 在生產環境常面臨「檢不到、排不准、壓不下、幻覺多」四大問題
- 長文本模型普及帶來新挑戰：上下文窗口大 ≠ RAG 效果好，需專門優化
- 優化投入產出比極高：重排序模型成本極低卻能顯著提升答案質量

## 出現在哪些內容

- [[Long-Context LLMs Meet RAG Overcoming Challenges for Long Inputs in RAG]]
- [[Daily/2026-07-12]]

## 相關概念

- [[Long-Context LLM RAG Integration]]
- [[Retrieval Reordering]]
- [[Context Engineering]]
- [[Hard Negative Mining]]
- [[RAG Evaluation]]
- [[Hybrid Search]]

## 更新紀錄

- 2026-07-12：首次建立。

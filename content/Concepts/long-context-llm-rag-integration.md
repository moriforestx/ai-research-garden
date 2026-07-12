---
type: concept
name: "Long-Context LLM RAG Integration"
date_updated: "2026-07-12"
tags:
  - concept
  - llm
  - rag
  - long-context
---

# Long-Context LLM RAG Integration

## 定義

超長上下文窗口（128K~2M+ tokens）大語言模型與檢索增強生成系統的深度融合架構模式。核心洞見：長文本窗口不能替代 RAG，但能改變 RAG 設計模式——從「檢索 Top-K 短段落」轉向「檢索長文檔 + 全文上下文 + 智能定位」。關鍵技術：上下文感知分塊、檢索重排序、迷失在中間現象緩解、引用級別檢索、生成式檢索。

## 為什麼重要

- Gemini 1.5 Pro（2M）、GPT-4.1（1M）、Claude 3.5（200K）等超長文本模型普及，重新定義 RAG 架構邊界
- 避免「將整個知識庫塞進上下文」的反模式，導致成本爆炸、延遲飆升、準確率下降
- 實現「長文本理解 + 精準檢索 + 可驗證生成」的最佳平衡點

## 出現在哪些內容

- [[Long-Context LLMs Meet RAG Overcoming Challenges for Long Inputs in RAG]]
- [[Daily/2026-07-12]]

## 相關概念

- [[RAG Optimization]]
- [[Retrieval Reordering]]
- [[Context Engineering]]
- [[Long-Context LLM]]
- [[Lost in the Middle]]
- [[Citation-Level Retrieval]]

## 更新紀錄

- 2026-07-12：首次建立。

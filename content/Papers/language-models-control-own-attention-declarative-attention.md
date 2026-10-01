---
title: "Language Models Can Control Their Own Attention"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-09-02"
organization: "KAIST AI / Google DeepMind"
source_url: "https://arxiv.org/abs/2609.02737"
date_collected: "2026-10-02"
date_updated: "2026-10-02"
tags:
  - ai
  - paper
---

# Language Models Can Control Their Own Attention

## 基本資訊

- 發布日期：2026-09-02
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2609.02737

## 概要

本文提出 Declarative Attention (DA) 協定，讓語言模型在思維鏈中宣告需關注的上下文區域，推理引擎據此解析注意力遮罩並跳過大部分 KV cache 讀取。DA 將生成劃分為三種模式：<global>（全上下文）、<focus>（特定區塊）、<local>（近期輸出）。跨 15 項長上下文任務的零樣本評測顯示，DA 在 Gemma-4-31B 與 Qwen-3.6-27B 上分別減少 52.0% 與 31.1% 的總關注 token，準確率僅下降 1.27pp 與 2.75pp，且隨模型規模擴大而縮小差距。

## 核心價值

零樣本、無需訓練即可實現稀疏注意力；模型自身產生注意力遮罩，推理引擎像解析工具調用般處理，大幅降低長上下文解碼的記憶體頻寬壓力。

## 應用情境與實務影響

適用於百萬 token 級長對話、RAG 檢索增強生成等場景；可直接套用於現有開源模型（Gemma、Qwen 等），無需重新訓練。

## 補充細節

arXiv:2609.02737v1 [cs.CL]，提交日期 2026-09-02。作者：Namgyu Ho (KAIST AI)、Tal Schuster (Google DeepMind)、Cicero Nogueira dos Santos (Google DeepMind) 等。

## 維護紀錄

- 收錄日期：2026-10-02
- 最後更新：2026-10-02

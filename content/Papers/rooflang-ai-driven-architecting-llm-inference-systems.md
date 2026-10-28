---
title: "RoofLang: Enabling AI-Driven Architecting of LLM Inference Systems"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-20"
organization: "Shanghai Xingyunzhili Artificial Intelligence Institute; Microsoft Research"
source_url: "https://arxiv.org/abs/2609.12551v2"
date_collected: "2026-10-29"
date_updated: "2026-10-29"
tags:
  - ai
  - paper
---

# RoofLang: Enabling AI-Driven Architecting of LLM Inference Systems

## 基本資訊

- 發布日期：2026-09-20
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.12551v2

## 概要

上海星雲智力 AI 研究院與 Microsoft Research 共同提出 RoofLang，一個領域專用語言 (DSL)，支援 AI 自主架構設計 LLM 推理系統。針對現有 AI 優化受限於 profiling 反饋、無法探索根本更優架構的問題，RoofLang 提供三大核心：(1) 通用圖表示 —— 以計算圖、硬體圖、放置映射建模負載與平台；(2) 語義保真變換空間 —— 圖重寫、分片、放置、通訊、記憶體決策為原語，保證功能等價；(3) 實現無關評估器 —— 基於屋頂線模型的離散事件模擬器，暴露算力、記憶體、網路、依賴、爭用、生命週期、容量成本。自主優化代理在 RoofLang 迴路中迭代搜尋，於 DeepSeek V4 Pro + NVIDIA B300 發現新架構，解碼吞吐與互動性雙提升 6.23–50.1%。另揭示 DeepSeek V4 系列得益於緊湊 KV-cache 設計，峰值解碼吞吐超其他模型 3.5–39.5×。代碼開源於 GitHub。

## 核心價值

首創「AI 自主架構設計迴路」：DSL 定義可驗證動作空間 + 模擬器提供實現無關反饋，讓 AI 從零設計並持續優化推理系統架構，突破固定軟體棧的優化天花板。

## 應用情境與實務影響

為 LLM 服務部署提供自動化架構探索工具，降低專家調優門檻；屋頂線模擬器可離線快速評估分片/放置/通訊策略，加速硬體採購決策；發現的模型級洞見（KV-cache 設計影響吞吐）指導模型架構選型。

## 補充細節

RoofLang 包含 Compute Graph（算子節點、張量邊、生命週期）、Hardware Graph（設備、互連、記憶體層級）、Placement（節點→設備映射）。語義保真變換含：算子融合、張量並行切分、流水線並行階段劃分、專家並行路由、KV-cache 卸載/複製、通訊拓撲重組。模擬器以離散事件推進，輸出 TTFT、解碼吞吐、記憶體佔用、互連利用率。自主代理以 LLM 為決策核心，結合模擬器反饋進行多輪搜尋。評測涵蓋 Llama-3、Qwen-2.5、DeepSeek V3/V4 等模型與 H100、B200、B300 硬體。

## 維護紀錄

- 收錄日期：2026-10-29
- 最後更新：2026-10-29

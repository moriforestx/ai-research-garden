---
title: "Evolving Infra: Agent-Adaptive LLM Serving at Scale"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-11-11"
organization: "UC Berkeley / MIT / NVIDIA / Georgia Tech"
source_url: "https://arxiv.org/abs/2611.12304"
date_collected: "2026-11-12"
date_updated: "2026-11-12"
tags:
  - ai
  - paper
---

# Evolving Infra: Agent-Adaptive LLM Serving at Scale

## 基本資訊

- 發布日期：2026-11-11
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2611.12304

## 概要

針對代理型工作負載（如並發編碼代理、電腦使用代理）提出 Evolving Infra，一個代理感知的 LLM 服務框架。核心創新在於解耦運算分配與 KV 快取管理：節點可在 prefill 與 decode 角色間無縫切換，同時保持共享主機記憶體 KV 池，配合線上規劃器與目錄追蹤活躍代理分支對快取區塊的引用。

## 核心價值

首創「計算角色與 KV 快取生命週期解耦」的服務架構，讓節點無需重啟即可動態適應代理工作負載的劇烈波動，大幅減少 KV 驅逐造成的重複計算。

## 應用情境與實務影響

大規模代理部署（Claude Code、電腦使用代理、程式碼生成管線）直接受益；雲端 LLM 服務商可參考此架構優化 prefill-decode 分離系統的資源利用率與尾部延遲。

## 補充細節

作者：Hao Kang、Weili Xu、Ziyang Li、Zheng Du、Hanchen Li、Tian Xia、Song Bian、Tushar Krishna、Huizi Mao、Ion Stoica、Song Han（來自 UC Berkeley、MIT、NVIDIA、Georgia Tech 等）。arXiv:2611.12304，2026年11月11日發布。在 Claude Code 126 併發代理實驗中，吞吐量達最佳靜態分割的 1.37 倍；啟用自適應分割僅降低 0.3% 吞吐量。對比 NVIDIA Dynamo，在編碼與電腦使用代理負載上顯著優於現有系統。

## 維護紀錄

- 收錄日期：2026-11-12
- 最後更新：2026-11-12

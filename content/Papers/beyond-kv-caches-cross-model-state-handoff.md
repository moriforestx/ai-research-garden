---
title: "Beyond K/V Caches: Cross-Model State Handoff in Hybrid Linear-Attention LLMs"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-11-07"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.08133"
date_collected: "2026-11-12"
date_updated: "2026-11-12"
tags:
  - ai
  - paper
---

# Beyond K/V Caches: Cross-Model State Handoff in Hybrid Linear-Attention LLMs

## 基本資訊

- 發布日期：2026-11-07
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2611.08133

## 概要

針對混合線性注意力 LLM（含循環狀態 REC 與卷積歷史 Conv），提出 Hybrid State Transfer (HST) 方法，實現跨模型的完整狀態遷移（K/V cache、REC、Conv），解決模型級聯、路由切換時需重新 prefill 的效率問題。

## 核心價值

首次完整解決混合架構 LLM 的跨模型狀態遷移，包含 K/V cache、循環狀態與卷積歷史，顯著降低模型切換開銷。

## 應用情境與實務影響

生產部署中透過模型級聯/路由平衡成本與品質的場景（長對話、即時助理、機器人控制）可直接受益；推動混合線性注意力架構在工業界的落地。

## 補充細節

作者：Jiacheng Cai、Tao Zhang、Siqi Liang、Yun Dai、Ziqian Zeng。arXiv:2611.08133v1，2026年11月7日發布。提出結構化 REC 映射與保持歷史順序的 Conv 對齊，經凍結目標模型輸出校準適配器。在 4B→27B 等模型對上驗證，mapper 速度比 re-prefill 快 2.7-25x，多輪遷移穩定。

## 維護紀錄

- 收錄日期：2026-11-12
- 最後更新：2026-11-12

---
title: "Hypic：面向混合注意力 LLM 服務的位置無關快取加速"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-12"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2607.01299"
date_collected: "2026-08-01"
date_updated: "2026-08-01"
tags:
  - ai
  - paper
---

# Hypic：面向混合注意力 LLM 服務的位置無關快取加速

## 基本資訊

- 發布日期：2026-07-12
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2607.01299

## 概要

提出 Hypic，針對混合注意力（Attention + Linear Attention）LLM 服務系統的位置無關快取（Position-Independent Caching, PIC）優化。現有 PIC 技術僅適用於純 Attention 或純 Linear Attention，無法處理混合堆疊。Hypic 設計段級自包含快取原語，支援跨層、跨注意力類型的 KV 狀態重用，在保持數值等價的前提下大幅降低預填與解碼階段的重複計算。於多款開源混合架構模型（如 GLA、RetNet、Mamba-2 混合版）實測，吞吐提升顯著、延遲下降。

## 核心價值

首個解決混合注意力架構 PIC 問題的系統級優化，填補服務引擎在新興架構上的加速空白，對部署長上下文、混合架構模型具直接效益。

## 應用情境與實務影響

服務引擎（vLLM、SGLang、TensorRT-LLM）可整合 Hypic 原語加速混合架構模型；長上下文、多輪對話、RAG 等大量重用前綴的場景受益最大；部署 GLA/RetNet/Mamba-2 等新架構時無需重寫快取邏輯。

## 補充細節

arXiv:2607.01299v2，提交於 2026-07-12（HTML 生成時間）。類別：cs.DC。作者機構含 NVIDIA 等。核心創新：段級自包含快取單元、跨注意力類型的位置無關狀態表示、相容現有連續批次與分頁 KV 快取基礎設施。實驗涵蓋多種混合架構與序列長度，展示預填階段計算量減少 30%+、解碼延遲顯著降低。

## 維護紀錄

- 收錄日期：2026-08-01
- 最後更新：2026-08-01

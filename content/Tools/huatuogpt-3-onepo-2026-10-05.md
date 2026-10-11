---
title: "HuatuoGPT-3：以單階段策略優化實現醫療領域 RL-only 適應，開源醫療 LLM 超越 GPT-6 Astra"
type: tool
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-05"
organization: "FreedomIntelligence"
source_url: "https://arxiv.org/abs/2610.05966"
date_collected: "2026-10-12"
date_updated: "2026-10-12"
tags:
  - ai
  - tool
---

# HuatuoGPT-3：以單階段策略優化實現醫療領域 RL-only 適應，開源醫療 LLM 超越 GPT-6 Astra

## 基本資訊

- 發布日期：2026-10-05
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2610.05966

## 概要

FreedomIntelligence 團隊提出 OnePO（One-stage Policy Optimization），透過自適應目標演化與教師退休機制，解決純 RL 領域適應中的冷啟動、梯度飢餓與教師分布錨定問題。僅用 20K 訓練樣本，OnePO 在 HealthBench (Total) 達 67.2，優於 SFT+RL（+2.7）與純 RL（+7.4）。進一步擴展產出 HuatuoGPT-3 開源醫療 LLM 系列，其 27B 版本在 HealthBench (Total) 達 70.1、HealthBench Professional 達 71.4，超越 GPT-6 Astra 等前沿閉源模型。模型權重、代碼與訓練數據開源於 GitHub。

## 核心價值

證明 RL-only 領域適應可超越傳統 SFT+RL 流程，單階段策略優化簡化訓練管線並提升探索多樣性；開源醫療 LLM 達到頂尖閉源模型水平，推動醫療 AI 普及。

## 應用情境與實務影響

為醫療、法律、金融等高專業領域提供低成本、高效能的領域適應範式；開源 27B 模型可直接部署於隱私敏感環境，支援臨床決策輔助、醫學教育、健康諮詢等應用。

## 補充細節

提交日期：2026-10-05 (v1)。方法：OnePO（Adaptive Objective Evolution + Teacher Retirement）。基礎模型：未公開，但從基礎模型直接 RL 適應。資料：20K 醫療樣本。基準：HealthBench Total 70.1、HealthBench Professional 71.4（27B 版）。開源位址：https://github.com/FreedomIntelligence/HuatuoGPT-3。模型系列：含多尺寸變體。ICML 2026 接收論文擴展版。

## 維護紀錄

- 收錄日期：2026-10-12
- 最後更新：2026-10-12

---
title: "TuringLLM: Efficiently Scaling Foundation Models Toward Physical AI"
type: paper
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-08-31"
organization: "Xpeng Inc. Foundation Model Team"
source_url: "https://arxiv.org/abs/2608.30567v1"
date_collected: "2026-10-29"
date_updated: "2026-10-29"
tags:
  - ai
  - paper
---

# TuringLLM: Efficiently Scaling Foundation Models Toward Physical AI

## 基本資訊

- 發布日期：2026-08-31
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://arxiv.org/abs/2608.30567v1

## 概要

Xpeng Foundation Model Team 發表 Turing-20B-A2B，一個 20B 參數的 Mixture-of-Experts 語言模型，每 token 僅激活約 2B 參數。模型採用 Quantile Routing 的動態 top-k 配置，實現 token 自適應專家分配並保持專家負載均衡；結合 Lightning Attention 與少量 full-attention 層的混合注意力架構，支援原生 128K 長上下文並透過 YaRN 推理時擴展至 512K。三階段漸進式預訓練課程（知識基礎、能力增強、品質退火）下，base-model 階段綜合能力超越 Qwen3-8B Base 並逼近 Qwen3.5-9B Base，兼顧長上下文表現與 prefill 延遲擴展效率，展示模型能力、長上下文擴展性與實務推理效率的有效平衡。

## 核心價值

提出可大規模部署於實體 AI 應用（自駕、具身智慧）的高效率 MoE 基礎模型架構，證明緊湊活躍參數預算下仍能達到一線開源模型水準。

## 應用情境與實務影響

為長上下文、低延遲的 Physical AI 場景（自駕感知推理、機器人即時決策）提供可直接部署的開源基礎模型選項；Quantile Routing 與 capacity-constrained prefill 設計可移植至其他 MoE 專案優化推理效率。

## 補充細節

模型採用 64 層、64 個專家（top-4 啟動）、隱藏維度 2048；預訓練 4.2T tokens。Quantile Routing 以 token 級動態門檻替代固定 top-k，解決專家負載不均問題；prefill 階段改用 capacity-constrained routing 降低專家間通訊開銷。長上下文採 4K→32K→128K 三階段延伸，推理時以 YaRN 外插至 512K。開源權重與推理代碼已發布於 GitHub。

## 維護紀錄

- 收錄日期：2026-10-29
- 最後更新：2026-10-29

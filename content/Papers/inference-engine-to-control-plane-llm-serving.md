---
title: "From Inference Engine to Inference Control Plane: Connecting vLLM, llm-d, and the Evolution of Efficient Distributed LLM Serving"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-23"
organization: "arXiv (systems synthesis)"
source_url: "https://arxiv.org/abs/2609.23130"
date_collected: "2026-10-19"
date_updated: "2026-10-19"
tags:
  - ai
  - paper
---

# From Inference Engine to Inference Control Plane: Connecting vLLM, llm-d, and the Evolution of Efficient Distributed LLM Serving

## 基本資訊

- 發布日期：2026-09-23
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.23130

## 概要

系統性綜述 LLM 推理服務架構演進，提出「推理引擎」與「推理控制平面」分層抽象：vLLM/SGLang/TensorRT-LLM 專注執行優化（調度、核心、量化、加速器後端），llm-d 控制平面負責分散式放置、KV 感知路由、預填/解碼解耦、多層 KV 管理、自動擴縮、異構引擎編排、預測延遲排程。論文綜合 2023-2026 學術與產業文獻，證實控制平面抽象已於 llm-d v0.8/v0.9 具體落地，並提出能源/碳感知、快取感知路由等研究議程。

## 核心價值

首次將 LLM 服務堆疊形式化為引擎/控制平面雙層架構，統一碎片化專案（vLLM、llm-d、NVIDIA Dynamo、SGLang）的設計空間，為生產級分散式推理提供架構藍圖與演進路線圖。

## 應用情境與實務影響

平台團隊可依循雙層抽象選型：引擎層比較 vLLM/SGLang/TensorRT-LLM 執行特性，控制平面層評估 llm-d/Dynamo 路由與編排能力；開源社群獲得標準化介面定義，利於引擎與控制平面獨立演進與互操作。

## 補充細節

arXiv:2609.23130v1 (2026-09-23)。作者綜合 llm-d Maintainers、Mitra et al.、Guy et al.、Liu & Kumar 等多組發布資料。涵蓋 vLLM PagedAttention、SGLang RadixAttention、TensorRT-LLM 編譯優化、NVIDIA Dynamo 解耦服務、llm-d v0.8/v0.9 架構演進、能源/碳感知排程等可驗證技術細節。

## 維護紀錄

- 收錄日期：2026-10-19
- 最後更新：2026-10-19

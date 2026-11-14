---
title: "跨部署堆疊優化 AI 推論：從模型服務到硬體協同的系統性分析"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-01"
organization: "多機構合作"
source_url: "https://arxiv.org/abs/2609.10550"
date_collected: "2026-11-14"
date_updated: "2026-11-14"
tags:
  - ai
  - paper
---

# 跨部署堆疊優化 AI 推論：從模型服務到硬體協同的系統性分析

## 基本資訊

- 發布日期：2026-07-01
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.10550

## 概要

arXiv:2609.10550 從全棧視角剖析 AI 推論優化，涵蓋模型壓縮（量化、蒸餾、剪枝）、運行時優化（連續批次、KV 快取複用、預填-解碼分離）、編譯器與核函式庫（TensorRT、Triton、XLA）、硬體感知排程（GPU/TPU/NPU 異構）、以及部署拓撲（單機多卡、多機叢集、邊緣協同）的聯動權衡。29 頁、12 張圖，系統性建立從模型到硬體的優化決策框架。

## 核心價值

提供部署堆疊各層的優化清單與決策矩陣，幫助團隊在延遲、吞吐、成本、精度四維度做有理據的取捨。

## 應用情境與實務影響

可直接作為 MLOps 平台建設、模型服務選型、硬體採購的技術參考；框架對齊 vLLM、SGLang、TensorRT-LLM、Triton 等主流棧。

## 補充細節

作者：Tejinder Singh, John Pflueger, Jeebak Mitra, Robert Lincourt, Mitchell Markow, Bhavesh A. Patel。提交於 2026-07-01。屬 cs.SE 與 cs.LG 交叉領域。

## 維護紀錄

- 收錄日期：2026-11-14
- 最後更新：2026-11-14

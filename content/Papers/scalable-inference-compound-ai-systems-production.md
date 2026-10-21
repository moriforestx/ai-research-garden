---
title: "複合 AI 系統的可擴展推理架構：Salesforce 百萬級日請求生產部署實證研究"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-04-25"
organization: "Salesforce AI Research"
source_url: "https://arxiv.org/abs/2604.25724"
date_collected: "2026-10-22"
date_updated: "2026-10-22"
tags:
  - ai
  - paper
---

# 複合 AI 系統的可擴展推理架構：Salesforce 百萬級日請求生產部署實證研究

## 基本資訊

- 發布日期：2026-04-25
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2604.25724

## 概要

Salesforce 研究團隊發表大規模生產部署實證研究，揭示支援 8,000+ 企業用戶、日均 72.2 萬次 LLM 推理、峰值 140 萬 RPS、跨 21 個全球區域、單月 1,360 億 tokens 的複合 AI 系統推理架構。論文系統分析異構模型後端編排、預填/解碼分離、PagedAttention 記憶體管理、多區域容災與自動擴縮容策略，獲 ACM CAIS 2026 接收。

## 核心價值

首個公開量化企業級複合 AI 系統（多模型編排、RAG、代理工作流）在百萬日請求規模下的完整架構與運維指標，為生產級 LLM 服務提供可複製的設計模式。

## 應用情境與實務影響

架構師可直接參考其預填/解碼分離、vLLM+PagedAttention 整合、全球多區域路由、容量規劃（2,250 RPS 佈署峰值）等實踐；運維團隊獲得具體的 SLO 監控指標、擴縮容觸發閾值、故障域隔離經驗。適用於構建企業級 AI 平台、代理服務編排層、多模型推理網關。

## 補充細節

論文編號：arXiv:2604.25724v1 (cs.DC; cs.LG)，2026-04-25 提交。獲 ACM Conference on AI and Agentic Systems (ACM CAIS 2026) 接收。核心貢獻：(1) 生產級複合 AI 系統參考架構：API 網關→編排層→異構推理後端（vLLM、DJL Serving、NVIDIA NIM）；(2) 預填/解碼分離顯著提升吞吐與尾延遲；(3) 全球 21 區域主動-主動部署，自動故障轉移 <30 秒；(4) 容量模型：峰值 2,250 RPS，日均 44 億 tokens；(5) 成本優化：批次排程、KV 快取共享、模型蒸餾級聯。開源實現組件部分釋出。作者單位：Salesforce AI Research。

## 維護紀錄

- 收錄日期：2026-10-22
- 最後更新：2026-10-22

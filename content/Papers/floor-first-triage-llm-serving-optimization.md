---
title: "Think Before You Grid-Search: Floor-First Triage for LLM Serving"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-08"
organization: "Taikang Insurance Group"
source_url: "https://arxiv.org/abs/2607.05876"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - paper
---

# Think Before You Grid-Search: Floor-First Triage for LLM Serving

## 基本資訊

- 發布日期：2026-07-08
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2607.05876

## 概要

Liu 於 2026 年 7 月 8 日發表 arXiv:2607.05876，提出 Floor-First Triage 方法論，重新定義 LLM 服務優化的分析流程。傳統做法在達不到延遲目標時大量跑基準、開啟重度分析器；本文主張先以解析式的「資源底板」——將每步解碼建模為 HBM 位元組、FLOPs、網路位元組、網路訊息、KV 容量五維資源向量，對同類資源求和、跨資源取最大得到樂觀底板、取總和得到悲觀底板。實測區間。若實測落入區間，說明重疊品質尚可；僅當殘差超過閾值才啟動分析器。部署替代方案以「牆面順序」比較：隨負載增長哪項資源最先觸及上限，而非單點基準。方法可組合：新注意力或狀態空間變體只需宣告一個模組，工具以零依賴計算器 + Agent 技能交付。案例分析 DeepSeek-V3.2 風格 671B MoE/MLA 模型於 16×H20 GPU：KV 容量牆將 TP16 並發限制在 ~70 請求（8K ctx）；稀疏注意力移除 KV 頻寬項但容量牆仍在；EP16+DP-Attention 佈局以微增同批次權重流量換取百倍容量牆（~644），單流延遲則 TP 優 2.4×。

## 核心價值

提供業界首個「先算底板、再跑基準」的系統化 LLM 服務優化工作流，將佈局選擇（TP vs EP+DP）從經驗主觀轉為可計算的營運點函數，大幅縮短調優週期與 GPU 成本。

## 應用情境與實務影響

MaaS 平台與企業自建推理集群可直接套用 Floor-First 計算器與 Agent 技能，在數分鐘內完成多佈局、多量化、多並行度的牆面順序排序，避免數百 GPU-hr 的盲目 Grid-Search；對 H20 等頻寬受限硬體特別高價值。

## 補充細節

作者：Yihua Liu（泰康保險集團）。v1 提交 2026-07-07，v2 更新 2026-07-08。主類 cs.PF（Performance），副類 cs.AI、cs.DC。開源零依賴 Python 計算器與 Agent 技能腳本，支援新模組聲明式擴充。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

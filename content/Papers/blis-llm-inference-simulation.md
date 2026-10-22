---
title: "BLIS：無需 GPU 的高保真 LLM 推理部署規劃模擬器"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-09"
organization: "多機構合作"
source_url: "https://arxiv.org/abs/2610.14255"
date_collected: "2026-10-23"
date_updated: "2026-10-23"
tags:
  - ai
  - paper
---

# BLIS：無需 GPU 的高保真 LLM 推理部署規劃模擬器

## 基本資訊

- 發布日期：2026-10-09
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2610.14255

## 概要

論文提出 BLIS，一個確定性、純 CPU 執行的離散事件模擬器，能完整建模 LLM 推理服務管線（准入、路由、排程、prefill/decode 執行、KV-cache 管理、搶佔）。BLIS 結合解析基函數與全局擬合的學習縮放係數，無需逐模型或逐 GPU 分析即可預測步驟延遲。跨 6 模型、3 種 GPU、36 實驗，BLIS 達到 6.7% 中位端到端誤差，速度比實機快約 200 倍。在 Llama-2-70B 的 420 種服務配置搜尋中，BLIS 找出符合 300ms 平均 TTFT SLO 的 4-GPU 部署，而競品工具需雙倍 GPU 或推薦失效配置。兩個完全在模擬中演化的策略（准入策略降關鍵級 TTFT P90 高達 82%、流控策略降過載負載 E2E P50 延遲 32-48%）已在真機驗證並併入開源分散式服務平台 llm-d。

## 核心價值

首個無需 GPU 即可高保真模擬完整推理管線的工具，將部署配置搜尋從昂貴的 GPU 叢集實驗轉移至 CPU 秒級模擬，並直接產出可上線的生產級策略。

## 應用情境與實務影響

大幅降低 LLM 生產部署的規劃成本與風險；團隊可在無 GPU 環境下快速評估硬體佈局、並行策略、排程政策與 SLO 滿足度，加速從原型到生產的落地。

## 補充細節

已獲 MLSys 2026 接收（DOI: 10.1145/3857382）；程式碼開源並整合至 llm-d 平台。作者涵蓋多機構研究人員。

## 維護紀錄

- 收錄日期：2026-10-23
- 最後更新：2026-10-23

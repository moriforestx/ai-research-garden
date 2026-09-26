---
title: "From Inference Engine to Inference Control Plane: Connecting vLLM, llm-d, and the Evolution of Efficient Distributed LLM Serving"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-19"
organization: "Boston University"
source_url: "https://arxiv.org/abs/2609.23130"
date_collected: "2026-09-27"
date_updated: "2026-09-27"
tags:
  - ai
  - paper
---

# From Inference Engine to Inference Control Plane: Connecting vLLM, llm-d, and the Evolution of Efficient Distributed LLM Serving

## 基本資訊

- 發布日期：2026-09-19
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.23130

## 概要

Boston University (Twinkll Sisodia) 發表的系統綜述與研究議程論文，追蹤 LLM 推理服務從單一引擎優化演進為分散式控制平面的架構轉變。核心論點：vLLM（執行引擎）與 llm-d/NVIDIA Dynamo（控制平面）為互補而非競爭關係——引擎優化單點執行，控制平面優化部署位置、時機、快取狀態、流量控制、自動擴縮容與異質硬體調度。論文證明現代推理瓶頸已從純 FLOPs 轉向「受管理的狀態、放置決策、網路移動與決策品質」。提出 Inference Execution Planner (IEP) 架構，需在聚合、prefill/decode、encode/prefill/decode 拓撲中選擇；整合快取來源與分層、轉移與重算、硬體變體、路由與準入策略、較慢的擴縮容動作。文獻證據分四層（同行審查、預印本、開源專案、雲端廠商生產報告），嚴格區分實驗結果與生產可行性。提出 9 大研究問題（RQ1-9），涵蓋圖式調度、狀態遷移、延遲預測、路由與擴縮容协同、異質容量抽象、可靠性整合、代理會話定價等。

## 核心價值

為 LLM 推理服務架構確立「引擎+控制平面」雙層範式，提供從學術研究到生產部署的完整證據綜合與未來 3-5 年系統演進路線圖。

## 應用情境與實務影響

直接指導企業級 LLM 推理平台（vLLM、SGLang、llm-d、NVIDIA Dynamo、KServe）架構選型與演進；對雲端廠商 GPU 叢集調度、代理/多模態工作負載服務、成本感知自動擴縮容、SLO 驅動路由具即時參考價值。

## 補充細節

arXiv:2609.23130v1 [cs.AI]，提交日期 2026-09-19。作者：Twinkll Sisodia (Boston University, twinklls@bu.edu)。License: CC BY 4.0。文獻範圍 2022-2026/09/13。關鍵引用：Orca、PagedAttention/vLLM、Splitwise、DistServe、Llundix、Mooncake、MemServe、Preble、NVIDIA Dynamo、llm-d v0.8/v0.9、AWS/OCI llm-d 生產研究。屬 AI Applications & Deployment 核心系統研究。

## 維護紀錄

- 收錄日期：2026-09-27
- 最後更新：2026-09-27

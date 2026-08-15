---
title: "Lodestar：面向異構叢集的線上學習 LLM 推理路由器"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-05-31"
organization: "學術與產業合作團隊"
source_url: "https://arxiv.org/abs/2606.00946"
date_collected: "2026-08-15"
date_updated: "2026-08-15"
tags:
  - ai
  - paper
---

# Lodestar：面向異構叢集的線上學習 LLM 推理路由器

## 基本資訊

- 發布日期：2026-05-31
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2606.00946

## 概要

針對大規模 LLM 推理部署中路由決策依賴靜態啟發式、難以適應異構硬體與動態負載的痛點，作者提出 Lodestar——首個線上學習式推理路由器。Lodestar 將路由建模為情境多臂老虎機問題，以請求特徵（前綴快取機會、排隊長度、GPU 利用率、KV cache 命中率等）為情境，即時更新路由策略，無需離線訓練資料。在包含多代 GPU（A100、H100、L40S）的異構叢集實測中，Lodestar 於約 5 分鐘線上學習後，平均 TTFT 降低 1.25–4.38×、P99 延遲降低 1.32–4.42×，顯著優於 Round-Robin、Least-Load、Prefix-Aware 等基線。

## 核心價值

首個證明「線上學習路由」在生產級異構 LLM 叢集可行的系統，解決離線訓練覆蓋率不足與分布漂移問題，為 Kubernetes 原生推理閘道（IGW）與 llm-d 等編排層提供可直接整合的智慧路由模組。

## 應用情境與實務影響

雲端服務商與企業可直接將 Lodestar 整合至 vLLM/SGLang/TGI 叢集前端，無需修改模型或推理引擎即可獲得自適應路由收益；對多租戶、多模型混部場景價值更大。

## 補充細節

論文編號 arXiv:2606.00946v1（2026-05-31 提交），屬 cs.DC（分散式、平行與叢集計算）。作者：Gangmuk Lim、Wanyu Zhao 等（學術與產業合作）。實驗平台：4 節點異構 GPU 叢集，模型混跑 Llama-3-70B、Qwen2-72B、Mixtral-8x7B；負載生成器模擬真實對話式流量（突發、長上下文、多輪）。程式碼將開源於對應 GitHub 倉庫。

## 維護紀錄

- 收錄日期：2026-08-15
- 最後更新：2026-08-15

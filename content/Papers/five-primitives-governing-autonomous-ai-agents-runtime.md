---
title: "Five Primitives for Governing Autonomous AI Agents at Runtime"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-08-27"
organization: "Aurite AI"
source_url: "https://arxiv.org/abs/2608.26696v1"
date_collected: "2026-10-29"
date_updated: "2026-10-29"
tags:
  - ai
  - paper
---

# Five Primitives for Governing Autonomous AI Agents at Runtime

## 基本資訊

- 發布日期：2026-08-27
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2608.26696v1

## 概要

Aurite AI 提出針對自主 AI 代理的運行時治理五大原語：Discovery（發現）、Identity（身份）、Governance（管控）、Attestation（證明）、Supply Chain（供應鏈）。論文指出企業部署自主代理時，現有為人類用戶與長期服務設計的 IAM、API Gateway、審計日誌等控制機制失效，因代理具三大特性：(1) Ephemeral —— 實例存活極短，無法依賴人工註冊；(2) Model-selected actions —— 行為由模型運行時決策，非預編碼，管控集合不可預知；(3) Discovered not provisioned —— 代理族群由 API 調用動態產生，非預置清單。五原語分別解決：發現什麼代理在嘗試什麼、可驗證身份於傳輸層呈現、行動前基於動態詞彙表拒絕默認、動作記錄哈希鏈簽名可第三方驗證、供應鏈信任決策一次作出持續消費。實作已四原語進入私有試營運，第五項為獨立工具待整合；架構代價含關鍵路徑延遲、每工作負載一 sidecar、失效即拒轉可用性事故為拒絕。

## 核心價值

將代理治理定義為運行時問題而非模型對齊或建置時問題，給出最小完備五原語分解與具體工程架構，填補企業級代理部署的安全治理空白。

## 應用情境與實務影響

為企業部署自主代理提供可落地的治理框架與風險評估基準；Identity 傳輸層呈現與 Attestation 哈希鏈設計可直接整合至現有 Zero Trust 架構；供應鏈信任鏈模型適用於模型版本漂移與依賴注入攻擊防禦。

## 補充細節

Discovery 採「聚合不追加、記名不記值」原則，區分可觀測性與治理；Identity 強調一主體多詞彙表、部分主體不可由存儲推導；Governance 採動態行為詞彙表與拒絕預設，支援運行中阻斷；Attestation 要求驗證者位於不同信任域、同時證明真實性與完整性；Supply Chain 強調組合包含非常規範疇、跨邊界歸因未解。作者提供 Agent Verifier 開源工具與 AgentRiskBOM 風險清單。

## 維護紀錄

- 收錄日期：2026-10-29
- 最後更新：2026-10-29

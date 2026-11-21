---
title: "Gateway API Inference Extension v1.6.2 釋出：Kubernetes 推理路由標準化"
type: tool
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-15"
organization: "Kubernetes SIG (WG-Serving / SIG-Network)"
source_url: "https://pkg.go.dev/sigs.k8s.io/gateway-api-inference-extension/api"
date_collected: "2026-11-22"
date_updated: "2026-11-22"
tags:
  - ai
  - tool
---

# Gateway API Inference Extension v1.6.2 釋出：Kubernetes 推理路由標準化

## 基本資訊

- 發布日期：2026-09-15
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://pkg.go.dev/sigs.k8s.io/gateway-api-inference-extension/api

## 概要

Kubernetes SIG 專案 Gateway API Inference Extension 於 2026 年 9 月 15 日發布 v1.6.2（Go module sigs.k8s.io/gateway-api-inference-extension/api）。此擴充套件利用 Envoy ext-proc 將支援 Gateway API 的閘道（Envoy Gateway、kgateway、GKE Gateway）升級為推理閘道，提供 InferencePool、InferencePoolImport 等 K8s 原生宣告式資源，支援模型感知路由、kv-cache 感知排程、LoRA 適配器路由、A/B 流量分割、藍綠部署與安全模型滾動升級。專案由 WG-Serving SIG-Network 主導，Apache-2.0 授權，已與 vLLM 合作加速 llm-d 整合。

## 核心價值

建立 Kubernetes 上生成式 AI 推理路由的廠商中立標準，解決自管模型的負載平衡、排程與生命週期管理難題，為生產級推理平台奠定共同基礎設施層。

## 應用情境與實務影響

平台團隊可透過標準 Gateway API 統一管理 vLLM、SGLang 等推理引擎；InferencePool 取代 Service 實現模型感知路由；支援 LoRA 熱插拔與金絲雀發布；Envoy Gateway、kgateway、GKE Gateway 等主流閘道已整合。

## 補充細節

Go pkg.dev 顯示 v1.6.2 於 2026-09-15 發布（Apache-2.0）。GitHub 倉庫 kubernetes-sigs/gateway-api-inference-extension 為官方原始碼。文檔站 gateway-api-inference-extension.sigs.k8s.io 完整說明 InferencePool、Endpoint Selection Extension、Inference-Aware Scheduling 等核心概念。Kubernetes 官方部落格 2025-06-05 發布專案介紹文。KubeCon NA 2026 設有「AI Inference + Agentic」專題軌，CNCF 於 2026-08 公布日程。

## 維護紀錄

- 收錄日期：2026-11-22
- 最後更新：2026-11-22

---
title: "vLLM v0.32.0 釋出：支援 NVFP4 KV Cache、Blackwell 原生優化、生產級穩定版"
type: tool
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-18"
organization: "vLLM Project (Sky Computing Lab, UC Berkeley)"
source_url: "https://github.com/vllm-project/vllm/releases/tag/v0.32.0"
date_collected: "2026-11-24"
date_updated: "2026-11-24"
tags:
  - ai
  - tool
---

# vLLM v0.32.0 釋出：支援 NVFP4 KV Cache、Blackwell 原生優化、生產級穩定版

## 基本資訊

- 發布日期：2026-10-18
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://github.com/vllm-project/vllm/releases/tag/v0.32.0

## 概要

vLLM 專案於 2026 年 10 月 18 日發布 v0.32.0 穩定版，為年度關鍵里程碑。核心亮點：(1) 原生支援 NVFP4 KV Cache，在 SM8x (Ampere)、SM90 (Hopper)、SM12x (Blackwell) GPU 上將 KV 快取量化至 4-bit，顯存佔用降低 75%，長文脈吞吐大幅提升；(2) 完整支援 NVIDIA Blackwell (B200/GB200) 架構，含 FP4 推理、Tensor Core 新指令集、NVLink 互聯優化；(3) 排程器引入 KV-cache watermark、雙階段跨組前綴快取命中、Marconi 風格準入策略、Mamba/線性注意力前綴保留，顯著降低搶佔與延遲抖動；(4) 量化生態擴充：2–7-bit 權重打包推理、Triton INT4 per-token-head KV 快取、AutoRound 線上量化、FP8 MoE 線上量化重構；(5) 927 次提交、389 位貢獻者，API 穩定性與文件同步強化。

## 核心價值

首個原生支援 Blackwell FP4/NVFP4 的開源推理引擎穩定版，將生產級 LLM 服務的單位成本推低至新基準，並確立 PagedAttention + 跨硬體平台（NVIDIA/AMD/Intel/TPU）的事實標準地位。

## 應用情境與實務影響

企業可在既有 H100 集群無縫啟用 NVFP4 省 3/4 KV 顯存、延遲不增；Blackwell 新採購即享 Day-0 優化；多模型共置、長文脈代理、推測解碼等進階部署模式開箱即用；Red Hat AI Inference Server、llm-d 等下游產品同步升級。

## 補充細節

後續 v0.33.0 於 11/2 釋出（PyTorch 2.14、CUDA 12.9、新模型 Day-0 支援 Kimi K3.1 Pro、Mistral Large 4）。GitHub Stars 達 96.6k，雙週釋出節奏。對比 SGLang v0.5.23 (11/2) 以 RadixAttention 擅長多輪前綴共享，vLLM 以生態廣、硬體支援全、長文脈穩定見長。

## 維護紀錄

- 收錄日期：2026-11-24
- 最後更新：2026-11-24

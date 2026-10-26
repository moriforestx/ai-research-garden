---
title: "vLLM 原生支援 Google TPU：TorchTPU 後端正式開源"
type: tool
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-20"
organization: "Google、Inferact、Meta PyTorch 團隊"
source_url: "https://developers.googleblog.com/announcing-new-vllm-and-sglang-inference-engines-on-tpu"
date_collected: "2026-10-27"
date_updated: "2026-10-27"
tags:
  - ai
  - tool
---

# vLLM 原生支援 Google TPU：TorchTPU 後端正式開源

## 基本資訊

- 發布日期：2026-10-20
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://developers.googleblog.com/announcing-new-vllm-and-sglang-inference-engines-on-tpu

## 概要

Google 與 Inferact 合作，於 2026 年 10 月 20 日在 PyTorch Conference 宣布 vLLM 原生支援 Google TPU。透過新開源的 TorchTPU 後端，vLLM 可在 TPU 上直接運行，支援前綴快取、推測解碼、分離式服務等核心功能。同步發布 SGLang TPU 後端。TorchTPU 由 Google 與 Meta PyTorch 團隊共建，讓 TPU 成為 PyTorch 原生裝置選項（含 GPU、CPU），模型服務無需更換推理引擎即可遷移硬體。

## 核心價值

首個將主流開源 LLM 推理引擎（vLLM、SGLang）原生移植至 TPU 的生產級方案，打破 GPU 鎖定、大幅擴展企業部署選擇。

## 應用情境與實務影響

企業可保留既有 vLLM/SGLang 服務碼，直接部署至 Google Cloud TPU 或自管 TPU 基礎設施；享有 TPU 價效優勢與生態系互通性。

## 補充細節

Google Developers Blog 正式公告（2026-10-20），同步宣布 TorchTPU 開源（GitHub: pytorch/torchtpu、google/torchtpu、pytorch/torchtitan、vllm-project/vllm）。vLLM 官方部落格同步發文「Introducing vLLM TorchTPU」（2026-10-19）。

## 維護紀錄

- 收錄日期：2026-10-27
- 最後更新：2026-10-27

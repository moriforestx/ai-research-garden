---
title: "BaseRT: Best-in-Class LLM Inference on Apple Silicon via Native Metal"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-01"
organization: "BaseCompute"
source_url: "https://arxiv.org/abs/2607.00501"
date_collected: "2026-08-06"
date_updated: "2026-08-06"
tags:
  - ai
  - paper
---

# BaseRT: Best-in-Class LLM Inference on Apple Silicon via Native Metal

## 基本資訊

- 發布日期：2026-07-01
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2607.00501

## 概要

推出 BaseRT，專為 Apple Silicon 打造的零依賴 C++ LLM 推理執行期，直接針對 Metal API 撰寫手工融合著色器，移除 MLX/PyTorch/CoreML 等中介層。在 Qwen3-0.6B、Llama-3.2 等模型上，解碼吞吐較 llama.cpp 提升 35%，預填吞吐提升 78%，並支援 2-bit 至 16-bit 量化格式。

## 核心價值

首個零中介層、晶片級核心庫的 Apple Silicon 專用 LLM 推理執行期，證明原生 Metal 實作可大幅超越現有跨平台方案。

## 應用情境與實務影響

讓 Mac/MacBook 成為高能效本地 LLM 推理平台，支援 Python/Node/Rust/Swift 綁定，適合隱私敏感、離線優先或邊緣部署場景。

## 補充細節

arXiv:2607.00501v1 [cs.CL]，2026-07-01 提交。作者：Prabod Rathnayaka, Fabian Waschkowski, Lukas Wesemann (BaseCompute)。程式碼開源於 GitHub，提供 C API 與多語言綁定。架構採資料驅動描述符、零配置解碼迴路、大量手寫 Metal 著色器。

## 維護紀錄

- 收錄日期：2026-08-06
- 最後更新：2026-08-06

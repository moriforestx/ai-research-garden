---
title: "NVIDIA 發布 Nemotron 3 Super：1200 億參數混合 Mamba-Transformer MoE 開放模型"
type: project
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-03-11"
organization: "NVIDIA"
source_url: "https://catalog.ngc.nvidia.com/orgs/nim/nvidia/containers/nemotron-3-super-120b-a12b-experimental/latest"
date_collected: "2026-08-25"
date_updated: "2026-08-25"
tags:
  - ai
  - project
---

# NVIDIA 發布 Nemotron 3 Super：1200 億參數混合 Mamba-Transformer MoE 開放模型

## 基本資訊

- 發布日期：2026-03-11
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://catalog.ngc.nvidia.com/orgs/nim/nvidia/containers/nemotron-3-super-120b-a12b-experimental/latest

## 概要

NVIDIA 於 2026 年 3 月 11 日在 GTC 大會發布 Nemotron 3 Super，為 Nemotron 3 系列第二款模型，採 120B 總參數 / 12B 啟用參數的混合 Mamba-Transformer MoE 架構（LatentMoE），支援原生 NVFP4 預訓練與多 Token 預測，並同步釋出模型權重、訓練資料與訓練配方。

## 核心價值

以混合架構兼顧長文脈效率與推理成本，並全棧開源（權重、資料、配方），降低大型 MoE 模型研究與部署門檻。

## 應用情境與實務影響

研究者可直接研究 120B 級 MoE 訓練細節；部署端透過 NVFP4 量化與 1M token 文脈窗，在單機或少量 GPU 上即可運行高品質長文脈代理任務。

## 補充細節

模型卡顯示 Hugging Face 與 NGC 同步於 2026-03-11 釋出。Nemotron 3 系列包含 Nano (31.6B, 2025-12-15)、Super (120.6B, 2026-03-11)、Ultra (~550B, 2026-06-04)。Super 於 Artificial Analysis Intelligence Index 得分 36.0，支援高達 1M token 文脸（BF16）。架構交替 Attention 與 Mamba-2 層，屬高效長文脈設計。

## 維護紀錄

- 收錄日期：2026-08-25
- 最後更新：2026-08-25

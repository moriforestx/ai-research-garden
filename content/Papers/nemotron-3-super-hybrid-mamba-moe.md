---
title: "Nemotron 3 Super: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-04-14"
organization: "NVIDIA"
source_url: "https://arxiv.org/abs/2604.12374"
date_collected: "2026-09-19"
date_updated: "2026-09-19"
tags:
  - ai
  - paper
---

# Nemotron 3 Super: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning

## 基本資訊

- 發布日期：2026-04-14
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2604.12374

## 概要

NVIDIA 發表 Nemotron 3 Super，一個 1200 億參數（活躍 120 億）的混合 Mamba-Attention Mixture-of-Experts 模型。該模型首創三大創新：1) 採用 NVFP4 精度預訓練，2) 引入 LatentMoE 架構優化每 FLOP 與每參數的準確度，3) 內建 MTP（Multi-Token Prediction）層支援原生推測式解碼加速。模型在 25 兆 tokens 上預訓練，經 SFT 與 RL 後訓練，支援高達 1M 上下文長度，在常見基準上達到可比準確度，推理吞吐量較 GPT-OSS-120B 提升 2.2 倍、較 Qwen3.5-122B 提升 7.5 倍。

## 核心價值

首個結合 LatentMoE、NVFP4 預訓練與 MTP 推測式解碼的開源混合架構大模型，實現極高推理效率與超長上下文。

## 應用情境與實務影響

模型權重、資料集與量化檢查點全數開源於 HuggingFace，可直接部署於生產環境；1M 上下文長度適合代理工作流、長文檔處理與複雜推理任務；高吞吐量降低推理成本。

## 補充細節

120B 總參數（12B 活躍），LatentMoE 專家設計，混合 Mamba-2 與稀疏全域 Attention 錨點，NVFP4 量化預訓練，25T tokens 預訓練資料，SFT+RL 後訓練，支援 1M context，HuggingFace 開源。

## 維護紀錄

- 收錄日期：2026-09-19
- 最後更新：2026-09-19

---
title: "Nemotron 3 Ultra: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-06-04"
organization: "NVIDIA"
source_url: "https://research.nvidia.com/labs/nemotron/files/NVIDIA-Nemotron-3-Ultra-Technical-Report.pdf"
date_collected: "2026-08-10"
date_updated: "2026-08-10"
tags:
  - ai
  - paper
---

# Nemotron 3 Ultra: Open, Efficient Mixture-of-Experts Hybrid Mamba-Transformer Model for Agentic Reasoning

## 基本資訊

- 發布日期：2026-06-04
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://research.nvidia.com/labs/nemotron/files/NVIDIA-Nemotron-3-Ultra-Technical-Report.pdf

## 概要

NVIDIA 於 2026 年 6 月 4 日發布 Nemotron 3 Ultra，550B 總參數（55B �� 活�躍）混合專家 Mamba-Transformer ��� � � 模型，���採用 LatentMoE、Multi-Token Prediction 和 NVFP4 量化，專為長運行 AI 代理設計。在 8k/64k token 設定下，相���較於 GLM-5.1-754B-A40B、Kimi-K2.6-1T-A32B 和 Qwen-3.5-397B-17B 分別達到 5.9x、4.8x、1.6x 高推���吞���吐量，並支援 1M tokens 上下文長度。

## 核心價值

結合 Mamba 的線性複���雜度、Transformer 的建模能力與 MoE 的參數效率，首次在 550B 規模���穩定���訓���練 NVFP4，為長上下文、高���吞���吐量、低成本的開源 LLM 設定新標���杆。

## 應用情境與實務影響

使單一 A100/H100 集群可部署 550B ��� � � 模型進行長代理������鏈推理；���訓���練食���譜與權重開源，降低前���沿 LLM 研究與開發門���檻；適合需要長上下文記���憶與複���雜推理的 AI 代理、工具使用與多步���驟任務場景。

## 補充細節

架構：混合 Mamba-Attention ��� � � 堆���疊 + LatentMoE + 兩頭 Multi-Token Prediction ��� � � 頭。���訓���練：NVFP4 量化預���訓���練 + PivotRL 對話工具使用數據 + SFT + RL + MOPD 後���訓���練。效能：AA-Omniscience ��� � � 基準分數 78.7；Hugging Face、ModelScope、OpenRouter、NVIDIA NIM 上可獲取。作者：NVIDIA Nemotron 團隊。論文 PDF ��� � � 包含完整架構、���訓���練細節與基準結果。

## 維護紀錄

- 收錄日期：2026-08-10
- 最後更新：2026-08-10

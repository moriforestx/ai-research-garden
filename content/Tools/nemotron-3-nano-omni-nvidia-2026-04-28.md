---
title: "Nemotron 3 Nano Omni：NVIDIA 釋出 30B 參數全模態 MoE 模型"
type: tool
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-04-28"
organization: "NVIDIA"
source_url: "https://huggingface.co/nvidia/Nemotron-3-Nano-Omni-30B-A3B-Reasoning-NVFP4"
date_collected: "2026-09-22"
date_updated: "2026-09-22"
tags:
  - ai
  - tool
---

# Nemotron 3 Nano Omni：NVIDIA 釋出 30B 參數全模態 MoE 模型

## 基本資訊

- 發布日期：2026-04-28
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://huggingface.co/nvidia/Nemotron-3-Nano-Omni-30B-A3B-Reasoning-NVFP4

## 概要

NVIDIA 於 2026 年 4 月 28 日發布 Nemotron 3 Nano Omni，採用 Mamba-Transformer 混合 MoE 架構（30B 總參數、3B 啟用參數），單一模型統一文本、圖像、視頻、音頻四大模態，支援 300K 上下文窗口與 16K 推理預算。模型在 build.nvidia.com、Hugging Face、NGC 同步開放，採 NVIDIA Nemotron Open Model License。arXiv:2604.24954 技術報告同步釋出。

## 核心價值

首個以 3B 算力成本實現全模態感知的開放 MoE 模型，Conv3D 視頻原生層與混合骨幹在單一推理循環完成跨模態推理，大幅降低企業級多模態代理部署門檻。

## 應用情境與實務影響

企業可單模型處理會議錄製、文檔智能、GUI/OCR、語音轉錄等富媒體工作流；開放權重與 NIM 部署路徑支援私有化與雲端彈性部署。

## 補充細節

架構亮點：Mamba2-Transformer Hybrid MoE、Conv3D 視頻時空建模、300K 上下文、16K 推理預算。基準測試顯示多模態理解準確率領先同級開放模型。Hugging Face: nvidia/Nemotron-3-Nano-Omni-30B-A3B-Reasoning-NVFP4。

## 維護紀錄

- 收錄日期：2026-09-22
- 最後更新：2026-09-22

---
title: "NVIDIA 發布 Nemotron 3.5 Super VL 與 Bolt 開源模型"
type: tool
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-10-15"
organization: "NVIDIA"
source_url: "https://blogs.nvidia.com/blog/nemotron-3-5-super-vl"
date_collected: "2026-11-01"
date_updated: "2026-11-01"
tags:
  - ai
  - tool
---

# NVIDIA 發布 Nemotron 3.5 Super VL 與 Bolt 開源模型

## 基本資訊

- 發布日期：2026-10-15
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://blogs.nvidia.com/blog/nemotron-3-5-super-vl

## 概要

NVIDIA 於 2026-10-15 正式發布 Nemotron 3.5 系列開源模型：Super VL（120B 參數 MoE、啟動 12B/token，混合 Mamba-Transformer 架構、支援多模態推理與工具使用）與 Bolt 74B-A9B 24GB（邊緣部署、2-bit 量化）、Bolt E4B 4GB（極致壓縮）。模型於 Hugging Face 開放權重，支援 llama.cpp、Ollama、vLLM 等推理框架。

## 核心價值

以單一開源多模態模型覆蓋從資料中心到邊緣裝置的代理部署全譜系，實現高吞吐、長上下文、工具使用與視覺推理的統一。

## 應用情境與實務影響

企業可在 DGX/RTX/本地筆電上部署同一模型族進行專用代理工作流；研究者獲得可客製化的 120B 級多模態基座，降低自建視覺語言模型門檻。

## 補充細節

Super VL 採 120B 參數 MoE、每 token 啟動 12B，混合 Mamba-Transformer 支援長上下文與多 token 預測 (MTP) 加速；在 PinchBench 同級開源模型中排名第一、BrowseComp 第二。Bolt 74B-A9B 以 2-bit 量化置入 24GB 顯存，Bolt E4B 4GB 針對 4GB 裝置優化。技術部落格同步發布架構細節與自訂指南。

## 維護紀錄

- 收錄日期：2026-11-01
- 最後更新：2026-11-01

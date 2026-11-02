---
title: "NVIDIA Nemotron 3.5 Lightning 與 NeMo Switchyard：針對長期代理 AI 工作負載的最高效開放模型"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-08-11"
organization: "NVIDIA"
source_url: "https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx"
date_collected: "2026-11-03"
date_updated: "2026-11-03"
tags:
  - ai
  - technical-development
---

# NVIDIA Nemotron 3.5 Lightning 與 NeMo Switchyard：針對長期代理 AI 工作負載的最高效開放模型

## 基本資訊

- 發布日期：2026-08-11
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://blogs.nvidia.com/blog/nemotron-lightning-switchyard-rtx-dgx

## 概要

NVIDIA 正式發布 Nemotron 3.5 Lightning，採用混合 Mamba-2 + Attention + MoE 架構，30B 總參數、3B 活躍參數、支援 1M token 上下文，專為長期運行的代理式 AI 工作負載優化。同步釋出 NeMo Switchyard 路由工具，讓開發者在邊緣裝置、PC、工作站、資料中心與雲端間靈活調度模型。模型採 OpenMDW-1.1 許可（允許商用），提供 BF16 與 NVFP4 量化檢查點，單張消費級/工作站級 GPU 即可運行。

## 核心價值

將百億級混合架構模型壓縮至單 GPU 可跑等級，並配套路由工具，大幅降低部署自主代理的門檻與成本。

## 應用情境與實務影響

適用於本地端代理部署、長對話 RAG、程式碼生成代理、邊緣推理等場景。開發者可透過 Ollama、Hugging Face、AWS SageMaker JumpStart、NVIDIA NIM 等多管道取得權重與推理服務。

## 補充細節

官方部落格發布於 2026-08-11，作者 Kari Briski。模型卡顯示訓練期間 2025-12 至 2026-05。Hugging Face 模型頁確認 Release Date 2026-08-11。Nemotron Coalition 成員提供評測方法論、推理軟體與資料集協助推進。基準測試顯示於長文本代理任務達同級最高效率。

## 維護紀錄

- 收錄日期：2026-11-03
- 最後更新：2026-11-03

---
title: "阿里巴巴釋出 Qwen3.8-27B 開放權重模型，支援原生多模態與百萬級上下文"
type: tool
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-08-14"
organization: "Alibaba (Qwen Team)"
source_url: "https://huggingface.co/Qwen/Qwen3.8-27B"
date_collected: "2026-09-21"
date_updated: "2026-09-21"
tags:
  - ai
  - tool
---

# 阿里巴巴釋出 Qwen3.8-27B 開放權重模型，支援原生多模態與百萬級上下文

## 基本資訊

- 發布日期：2026-08-14
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://huggingface.co/Qwen/Qwen3.8-27B

## 概要

阿里巴巴於 2026 年 8 月 14 日釋出 Qwen3.8-27B 開放權重模型，採 Apache 2.0 授權。此為密集型 270 億參數原生多模態模型（支援文字、圖像、視訊、圖表、文件輸入），原生上下文窗口 262,144 tokens，可透過 YaRN 延伸至 100 萬 tokens。具備可配置的 reasoning_effort 模式以調整思考深度節省算力。ModelScope 元資料記錄釋出時間為 2026-08-14 15:00 UTC，Hugging Face 倉庫同步上線。

## 核心價值

首個在 Apache 2.0 下釋出的原生多模態密集型 27B 模型，提供免收入分成門檻的自架選項，支援百萬級長上下文與可調推理深度，為開發者與企業提供高自由度的前沿模型基座。

## 應用情境與實務影響

開發者可直接在消費級/企業級 GPU 上部署（量化後約 14-16 GB VRAM），適用於程式碼生成、辦公文件處理、多模態問答等場景；長上下文能力適合大規模文件分析與代理人記憶體；Apache 2.0 允許商業化衍生與再授權，降低供應鏈鎖定風險。

## 補充細節

Qwen3.8 世代包含 MoE 旗艦 Qwen3.8-Max（2.4 兆參數，8/3 發布 API）與密集型 Qwen3.8-27B（8/14 開放權重）。架構採 48 層 Gated DeltaNet + 16 層全注意力混合設計，原生多模態對齊而非事後拼接。基準測試顯示程式碼與辦公場景超越 Qwen3.7-Plus。同期競品：GLM-5.3（Z.ai，8/14）、Gemini 3.7 Flash（Google，8/13）、Grok 4.6（xAI，8/12）。來源：Hugging Face 模型卡、ModelScope 元資料、OrcaRouter 釋出追蹤、Kingy.ai 規格分析、ITHome 報導、Wikipedia Qwen 條目。

## 維護紀錄

- 收錄日期：2026-09-21
- 最後更新：2026-09-21

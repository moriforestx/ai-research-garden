---
title: "Qwen3.8-27B"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-08-14"
organization: "Alibaba Qwen"
source_url: "https://huggingface.co/Qwen/Qwen3-8-27B"
date_collected: "2026-08-28"
date_updated: "2026-08-28"
tags:
  - ai
  - technical-development
---

# Qwen3.8-27B

## 基本資訊

- 發布日期：2026-08-14
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://huggingface.co/Qwen/Qwen3-8-27B

## 概要

Alibaba 的 Qwen 團隊於 2026 年 8 月 14 日發布 Qwen3.8-27B，這是一個開放權重的視覺語言模型，採用 Apache 2.0 授權。模型具有 270 億個參數（含視覺編碼器則為 280 億），採用混合架構（48 層 Gated DeltaNet 線性注意力 + 16 層完整注意力），原生支援 262,144 tokens 長度的上下文窗口，可透過 YaRN 擴展至 1M tokens。支援文字、圖像和影像作為輸入，單張 24GB 顯卡即可以 4-bit 量化運行。在代理工作（編碼、辦公任務、桌面/行動控制）方面表現優於 Claude Opus 4.6 Max，但在知識密集型推理上則略遜一籌。

## 核心價值

開放權重的 27B 多模態模型，在單卡消費級硬體上即能達成接近頂尖閉源模型的代理任務表現，降低了進階 LLM 的使用門檻。

## 應用情境與實務影響

開發者可在本地工作站上部署並微調此模型，用於編程助手、文件處理與多媒體理解等場景；企業可作為成本效益高的自托管 LLM 方案。

## 補充細節

模型在 Hugging Face 上提供完整權重與授權文件，社區已釋出 GGUF 量化版本供 LM Studio 等工具使用。基準測試顯示其在 Agentic 任務中排名前十，特別適合用於程式碼生成、瀏覽器自動化與桌面操作工作流。

## 維護紀錄

- 收錄日期：2026-08-28
- 最後更新：2026-08-28

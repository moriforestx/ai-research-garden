---
title: "NVIDIA 發布 Nemotron 3.5 Super VL：120B 參數開放權重視覺語言模型，支援百萬 Token 上下文"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-16"
organization: "NVIDIA"
source_url: "https://developer.nvidia.com/blog/nvidia-nemotron-3-5-super-vl-powers-specialized-agents-with-multimodal-reasoning"
date_collected: "2026-11-13"
date_updated: "2026-11-13"
tags:
  - ai
  - tool
---

# NVIDIA 發布 Nemotron 3.5 Super VL：120B 參數開放權重視覺語言模型，支援百萬 Token 上下文

## 基本資訊

- 發布日期：2026-10-16
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://developer.nvidia.com/blog/nvidia-nemotron-3-5-super-vl-powers-specialized-agents-with-multimodal-reasoning

## 概要

NVIDIA 於 2026 年 10 月 16 日發布 Nemotron 3.5 Super VL，一個 120B 總參數（12B 啟動參數）的混合專家架構視覺語言模型。模型結合 Mamba-2、MoE 與注意力層，整合 C-RADIO 視覺編碼器，原生支援文字、圖像、文件與視頻輸入，上下文窗口達 1M tokens。採用多教師在線策略蒸餾（MOPD）從 Nemotron 3 Ultra 蒸餾而來，保留編程能力並強化視覺推理、工具使用與長視頻理解。以開放權重形式在 Hugging Face 釋出（BF16、NVFP4 格式），並提供 NGC 容器部署。

## 核心價值

首個在單一模型中統合推理、指令遵循、工具使用與多模態（文本/圖像/文件/視頻）理解的開放權重百萬上下文視覺語言模型，為專業代理人工作流提供原生部署路徑。

## 應用情境與實務影響

開發者可直接使用開放權重進行領域適配、量化或全精度推理；企業可透過 NGC 容器快速部署；單 GPU 即可達成同級開放模型 5 倍吞吐量，大幅降低多模態代理人系統的推理成本。適用於文件智能、視頻理解、代碼生成與工具調用等代理人任務。

## 補充細節

NVIDIA Technical Blog 於 2026-10-16 發布技術詳解。模型於 2026-10-15 在 Hugging Face 釋出權重。架構為交錯 Mamba-2、MoE 與注意力層，120B 總參數、12B 啟動參數。視覺編碼器採用 C-RADIO，支援圖表、表格、OCR、多頁文件與視頻理解。兩階段 SFT 管線結合視覺證據與推理、對話、安全、長上下文與代理人軌跡數據。授權為 NVIDIA 開放模型許可條款，允許商業與非商業使用。

## 維護紀錄

- 收錄日期：2026-11-13
- 最後更新：2026-11-13

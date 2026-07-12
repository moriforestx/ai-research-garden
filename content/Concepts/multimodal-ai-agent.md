---
type: concept
name: "Multimodal AI Agent"
date_updated: "2026-07-12"
tags:
  - concept
  - multimodal
  - ai-agent
  - nvidia
---

# Multimodal AI Agent

## 定義

原生支援文本、圖像、音頻、視頻等多模態輸入輸出，能夠在單一推理過程中跨模態推理、規劃、執行工具的智能體。區別於「多模態模型 + 文本 Agent」的串聯架構，真正的多模態 Agent 具備：統一 Token 空間、跨模態注意力機制、多模態工具調用（如視覺檢索、音頻生成）、多模態記憶管理。代表系統：NVIDIA Nemotron 3 Nano Omni、Google Gemini 3.5/4、OpenAI GPT-5.5、Anthropic Claude Opus 4.6。

## 為什麼重要

- 現實世界本質上是多模態的，單模態 Agent 無法處理「看圖說話、聽聲音找圖、看視頻寫代碼」等複合任務
- 邊緣部署需求推動輕量化多模態模型（Nano Omni、Gemma 4 12B）發展，使消費級設備能運行本地多模態 Agent
- 多模態能力是通用人工智能（AGI）的必要條件之一

## 出現在哪些內容

- [[Nemotron 3 Nano Omni]]
- [[Daily/2026-07-12]]

## 相關概念

- [[Vision Transformer Spatial Priors]]
- [[Voice Agent]]
- [[Multimodal Foundation Model]]
- [[Edge AI Deployment]]
- [[Unified Token Space]]

## 更新紀錄

- 2026-07-12：首次建立。

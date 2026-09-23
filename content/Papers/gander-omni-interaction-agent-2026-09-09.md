---
title: "Omni Interaction Agent Technical Report: Gander - A Cerebellum-Brain Collaborative Framework for End-to-End Multimodal AI Agents"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-09-09"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2609.08977"
date_collected: "2026-09-24"
date_updated: "2026-09-24"
tags:
  - ai
  - paper
---

# Omni Interaction Agent Technical Report: Gander - A Cerebellum-Brain Collaborative Framework for End-to-End Multimodal AI Agents

## 基本資訊

- 發布日期：2026-09-09
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2609.08977

## 概要

提出 Gander，一種端到端的全模態 AI 代理人架構，透過小腦-大腦協作框架和區塊級 token 串流設計，統一全模態感知、即時互動與代理人推理能力。小腦處理低延遲的實時互動（感知、輪流切換、語音生成），大腦負責較慢的高階推理與代理人任務執行，兩者透過工具呼叫與編排運行時持續交互。此設計使得使用者可在模型思考過程中隨時中斷並重新導向，而模型亦能主動提供回饋，實現真正的全雙工多模態對話與非同步長時程代理人執行。

## 核心價值

首次提出感知與認知的雙軌道架構於端到端 AI 代理人中，解決傳統輪流制模型在實時互動與深度推理間的根本矛盾，為真正自然的多模態人機協作奠定基礎。

## 應用情境與實務影響

適用於需要即時回應與深度推理的場景：客服機器人、程式設計夥伴、科學研究助理等；支援真正的全雙工語音對話；降低因模型思考導致的互動遲頓問題。

## 補充細節

論文於 2026-09-09 提交至 arXiv (ID: 2609.08977v3)。Gander 架構包含兩個核心設計：(1) 小腦-大腦協作框架：小腦（前小腦）負責實時多模態感知與互動，處理音訊、視訊、文字等串流輸入；大腦（後大腦）負責複雜推理、規劃與代理人任務執行，如程式設計、資料檢索、檔案操作等；(2) 區塊級 token 串流設計：將輸入與輸出 flatten 為有序 token 串流，在區塊層級進行處理，使得小腦與大腦可持續交互而非傳統的輪流制。在對話能力、互動能力、理解力與工具輔助任務執行四個維度上進行評估。內部人類評估顯示 Gander 維持自然且富有表達力的語音對話；基準測試展現有效的輪流控制能力及令人鼓舞的語音問答與理解表現。模型支援在思考過程中被中斷、重新導向視線或展示畫面，同時能夠 volunteer 資訊或建議而不需等待提示。此工作为突破傳統 LLM 代理人的交互限制提供了創新架構，為真正自然的多模態人機協作系統開闢新方向。

## 維護紀錄

- 收錄日期：2026-09-24
- 最後更新：2026-09-24

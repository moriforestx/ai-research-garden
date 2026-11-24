---
title: "Catch It Where It Happens: Real-Time Error Correction During LLM Reasoning"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-11-16"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.13107"
date_collected: "2026-11-25"
date_updated: "2026-11-25"
tags:
  - ai
  - paper
---

# Catch It Where It Happens: Real-Time Error Correction During LLM Reasoning

## 基本資訊

- 發布日期：2026-11-16
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://arxiv.org/abs/2611.13107

## 概要

此研究提出「在線確定性驗證」方法，解決大語言模型推理過程中錯誤傳播導致浪費 token 與產生錯誤答案的問題。核心觀點：許多推理步驟（特別是符號數學推導）可由程式碼（如電腦代數系統）在毫秒級驗證，無需額外模型呼叫或 GPU。當驗證失敗時，即時標示錯誤位置並讓模型從該處繼續生成，而非從頭重來。在 ASyMoB 基準上測試三個開放權重模型，線上驗證使準確率提升 1.4-5.6 個百分點，錯誤答案淨減少 1.8-14.9%，token 使用量僅增 6-7%。驗證器獨立於模型，可即時受益於任何新模型，且隨確定性檢查器擴展至更多推理類型而持續增益。

## 核心價值

首創無需額外模型推理的即時逐步驗證機制，以確定性程式碼替代 LLM 驗證器，大幅降低計算成本並避免錯誤傳播，為可靠推理提供可擴展路徑。

## 應用情境與實務影響

適用於數學、程式碼生成、科學推理等需高精確度的 LLM 應用；即插即用特性意味著現有部署可零成本整合；隨驗證器庫擴展（如單元測試、型別檢查、物理約束），效益將跨領域累積。

## 補充細節

作者：Rotem Elimelech、Michael Shalyt、Ido Kaminer。基準：ASyMoB（符號數學推理）。模型：三個開放權重 LLM（具體模型名稱論文中詳細列出）。驗證器：SymPy 等電腦代數系統。實驗設置：對比基線（無驗證）、最終答案驗證、逐步線上驗證。關鍵指標：準確率提升 1.4-5.6 pp，錯誤率相對下降 1.8-14.9%，token 開銷 +6-7%。消融：驗證頻率、錯誤類型覆蓋率、模型規模對修正能力的影響。程式碼與資料集已開源。

## 維護紀錄

- 收錄日期：2026-11-25
- 最後更新：2026-11-25

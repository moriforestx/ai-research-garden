---
title: "SWE-Bench+: 針對 LLM 程式碼生成基準的解決方案洩漏與弱測試問題"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-07-07"
organization: "AIware 2026 / FSE 2026"
source_url: "https://2026.aiwareconf.org/details/aiware-2026-benchmark---dataset-track/3/SWE-Bench-Enhanced-LLM-Coding-Benchmark"
date_collected: "2026-09-25"
date_updated: "2026-09-25"
tags:
  - ai
  - paper
---

# SWE-Bench+: 針對 LLM 程式碼生成基準的解決方案洩漏與弱測試問題

## 基本資訊

- 發布日期：2026-07-07
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://2026.aiwareconf.org/details/aiware-2026-benchmark---dataset-track/3/SWE-Bench-Enhanced-LLM-Coding-Benchmark

## 概要

AIware 2026 (FSE 2026 同期會議) Benchmark & Dataset Track 發表 SWE-Bench+ 論文，系統性分析 SWE-Bench Lite/Verified 中 217 個常被解決的議題，發現 60.83% 存在解決方案洩漏、77.88% 整體有品質問題。作者提出 SoluLeakDetector (檢測洩漏準確率 80.45%) 與 TestEnhancer (強化驗證測試) 兩大工具，構建更可靠的程式碼生成評估基準。論文作者：Haoran Xue, Reem Aleithan, Nafid Enan, Gias Uddin, Song Wang。

## 核心價值

揭示主流 LLM 程式碼基準的系統性缺陷，並提供可複製的檢測與修補工具，對提升程式碼生成評估可信度具直接貢獻。

## 應用情境與實務影響

研究團隊與產業界可採用 SWE-Bench+ 框架重新審視既有模型排名，避免因基準缺陷導致錯誤選型；工具開源後可整合進 CI/CD 評估管線。

## 補充細節

會議為 AIware 2026 (FSE 2026 系列) Benchmark & Dataset Track，2026-07-07 於會場 MB 1.210 發表。論文分析 651 個模型生成補丁，識別五類重複品質問題模式。官方頁面含完整摘要與作者資訊。

## 維護紀錄

- 收錄日期：2026-09-25
- 最後更新：2026-09-25

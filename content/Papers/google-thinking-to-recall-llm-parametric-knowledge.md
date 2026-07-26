---
title: "Thinking to Recall: How Reasoning Unlocks Parametric Knowledge in LLMs"
type: paper
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-06-24"
organization: "Google Research"
source_url: "https://research.google/blog/thinking-to-recall-how-reasoning-unlocks-parametric-knowledge-in-llms"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - paper
---

# Thinking to Recall: How Reasoning Unlocks Parametric Knowledge in LLMs

## 基本資訊

- 發布日期：2026-06-24
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://research.google/blog/thinking-to-recall-how-reasoning-unlocks-parametric-knowledge-in-llms

## 概要

Google Research 於 2026 年 6 月 24 日發表論文《Thinking to Recall: How Reasoning Unlocks Parametric Knowledge in LLMs》（arXiv:2603.09906），揭示推理機制在大型語言模型中對單跳事實問答的意外幫助。實驗針對 Gemini-2.5 Flash/Pro 與 Qwen3-32B，在 SimpleQA Verified 與 EntityQuestions 閉卷問答基準上，啟用推理後 pass@k 顯著提升，甚至能回覆關閉推理時幾乎無法觸及的正確答案。研究發現兩大機制：(1) 計算緩衝效應——生成額外 token 提供額外前向傳遞，即便內容無意義（如重複 "Let me think"）仍能改善回溯；(2) 事實啟動——模型自發產生相關事實作為語義橋樑，促使目標事實被提取，但若中間事實出現幻覺會顯著降低最終答案正確率。據此提出測試時選策略：產生多條推理軌跡、保留無幻覺者，可大幅提升準確率。

## 核心價值

證明推理不只是分解複雜任務，更能擴展 LLM 參數記憶的可觸及邊界；事實啟動機制雙面性強——正確中間事實助益、錯誤中間事實有害，為程序獎勵訓練提供新方向。

## 應用情境與實務影響

模型提供商可在推理階段實作無幻覺軌跡篩選，或在 RL 訓練中引入過程獎勵鼓勵事實支撐的中間步驟，直接降低閉卷問答幻覺率；開源社群可依此設計更穩健的推理蒸餾管線。

## 補充細節

論文已被 COLM 2026 接收。實驗使用 pass@k 指標量化參數記憶邊界，對比推理開/關兩種模式。計算緩衝實驗以無意義重複字串控制語義內容；事實啟動實驗以嚴格過濾提取純事實片段。審計管線以搜尋增強驗證器逐條檢核數十萬推理軌跡的中間事實正確性。作者：Zorik Gekhman、Roee Aharoni、Eran Ofek、Mor Geva、Roi Reichart、Jonathan Herzig（Google Research）。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

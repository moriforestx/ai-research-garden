---
title: "Free Lunch Uncertainty：序列層級 Rényi Entropy 讓 LLM 推理不確定性量化零成本"
type: paper
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-11-13"
organization: "Independent researchers"
source_url: "https://arxiv.org/html/2611.13414v1"
date_collected: "2026-11-15"
date_updated: "2026-11-15"
tags:
  - ai
  - paper
---

# Free Lunch Uncertainty：序列層級 Rényi Entropy 讓 LLM 推理不確定性量化零成本

## 基本資訊

- 發布日期：2026-11-13
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://arxiv.org/html/2611.13414v1

## 概要

arXiv:2611.13414（2026-11-13 提交）提出 Free Lunch Uncertainty 方法，利用 Sequential Monte Carlo (SMC) 粒子解碼過程中產生的粒子集，零額外計算成本地估算序列層級 Rényi Entropy（SREβ），解決傳統需多次獨立採樣計算 Shannon Entropy 的高昂開銷。理論證明 Rényi Chain Rule 將序列熵分解為逐步累加，並在數學、代碼、邏輯推理基準上驗證：SREβ 比單純 log-probability 更能區分正確與錯誤推理路徑，且計算開銷可忽略不計。

## 核心價值

首個「免費午餐」級不確定性量化方法：在解碼過程中順手取得序列層級 Rényi Entropy，無需額外前向傳播或採樣，大幅降低生產級 LLM 可靠性監控門檻。

## 應用情境與實務影響

部署端可即時監控 LLM 推理品質、觸發人工介入或自動重試；對程式生成、數學推理、代理式工作流等高風險場景具即時防護價值。開放原始碼與預註冊實驗設計強化可重現性。

## 補充細節

作者：Erfan Baghaei Potraghloo 等。跨列 cs.LG、cs.CL、cs.AI。SREβ 定義為累積負對數 power mean，β 控制對尾部分佈敏感度。實驗顯示 β=2 時在 GSM8K、MBPP、HumanEval 上 AUC 顯著優於 predictive entropy、log-prob 等基線。

## 維護紀錄

- 收錄日期：2026-11-15
- 最後更新：2026-11-15

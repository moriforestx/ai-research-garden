---
title: "Dream-RSI: Recursive Self-Improvement through Evolving Worlds"
type: paper
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-09-14"
organization: "Google DeepMind"
source_url: "https://arxiv.org/abs/2609.14858"
date_collected: "2026-10-30"
date_updated: "2026-10-30"
tags:
  - ai
  - paper
---

# Dream-RSI: Recursive Self-Improvement through Evolving Worlds

## 基本資訊

- 發布日期：2026-09-14
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://arxiv.org/abs/2609.14858

## 概要

Google DeepMind 發表 Dream-RSI，建立遞迴自我改進迴路：代理人在線上探索收集發現歷史，將歷史轉換為可重播模擬器，透過「做夢」離線優化元探索策略，再重新部署升級後的策略。此方法在編碼基準測試上以 162 倍更少的搜尋呼叫達成同等效能，且不需修改底層模型權重。

## 核心價值

證明可在不重新訓練模型權重的前提下，透過探索層的自我改進迴路大幅提升代理人效率，為 AI 代理人的長期自主進化提供新範式。

## 應用情境與實務影響

適用於程式碼生成、自動化研究、機器人控制等需長時程探索的任務；可降低部署代理人時的推理成本與搜尋開銷。

## 補充細節

arXiv:2609.14858v2 (2026-10-06 更新)。17 位作者來自 Google、Google DeepMind、馬里蘭大學與維吉尼亞大學。配套 GitHub 專案：https://github.com/zhengkid/Dream-RSI。核心創新在於將探索歷史轉為可微分模擬器，讓策略在離線環境快速迭代。

## 維護紀錄

- 收錄日期：2026-10-30
- 最後更新：2026-10-30

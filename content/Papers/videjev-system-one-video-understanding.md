---
title: "VideoJev: System One Model for Video Understanding and Interaction"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-10-13"
organization: "Nanjing University (MCG-NJU)"
source_url: "https://arxiv.org/abs/2610.18615"
date_collected: "2026-11-08"
date_updated: "2026-11-08"
tags:
  - ai
  - paper
---

# VideoJev: System One Model for Video Understanding and Interaction

## 基本資訊

- 發布日期：2026-10-13
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2610.18615

## 概要

南京大學 MCG 團隊提出 VideoJev，一種「System One」視頻理解模型家族，統一時域定位與多選視頻問答，採用共享候選評分介面，直接評估時間區間與文本選項而無需自回歸生成，實現 >100x 問答加速。開源 4B 與 35B-A3B 兩個版本，模型權重發布於 Hugging Face 與 ModelScope，代碼開源於 GitHub。

## 核心價值

首創將視頻理解框架為無生成式的候選評分任務，大幅降低推理延遲並保持高精度，為即時視頻交互應用奠定基礎。

## 應用情境與實務影響

適用於需要即時視頻決策的場景：自動駕駛感知、手術機器人視覺導航、工業檢測流水線、即時安防監控、具身智能體視覺閉環。開源權重與代碼降低部署門檻。

## 補充細節

論文編號 arXiv:2610.18615v1，分類 cs.CV。作者 Yuhan Zhu 等。核心創新：(1) 共享候選評分統一 grounding 與 QA；(2) 視覺計算緩存重用應對連續查詢；(3) 開源兩種規模模型（4B 密集、35B-A3B MoE），在多項基準達到 SOTA。

## 維護紀錄

- 收錄日期：2026-11-08
- 最後更新：2026-11-08

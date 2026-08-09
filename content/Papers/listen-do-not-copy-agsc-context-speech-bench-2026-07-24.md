---
title: "Listen, Do Not Copy: Internalizing Audio-Grounded Scaffold Context for Robust Omni-Model Speech Understanding"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-07-24"
organization: "�獨立研究團隊 (來自 arXiv 提交)"
source_url: "https://arxiv.org/abs/2607.21943"
date_collected: "2026-08-10"
date_updated: "2026-08-10"
tags:
  - ai
  - paper
---

# Listen, Do Not Copy: Internalizing Audio-Grounded Scaffold Context for Robust Omni-Model Speech Understanding

## 基本資訊

- 發布日期：2026-07-24
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2607.21943

## 概要

該論文於 2026 年 7 月 24 日在 arXiv 發表，提出「感知���繞過」(perception bypass) 現象：模型可透過含答案的上下文直接得分，而非實際處理音���訊。為解決此問題，研究團隊提出 AGSC (Audio-Grounded Scaffold Context) 自動合成管線與 Context-Speech Bench (CSB)，並透過有監督���訓���練與 GDPO ��� � � 階段實現內部化(internalization)，使模型在去除線索後仍能保持強 robustness。在重���疊���噪音場景中，無線索 mpWER 從 25%–71% 下降至 9%–15%。

## 核心價值

首次系統化定義並���測量語音模型的「感知���繞過」問題，提出可移除的���訓���練線索機制 (AGSC) ��� � � 與基準 (CSB)，���顯著提升模型在真實���雜���訊環境中的語音理解���穩定性，而非依���賴上下文投機取���巧。

## 應用情境與實務影響

改進語音助理、會議記錄、多模態 AI 等在���嘈���雜環境中的可���靠性；提供可一般化的���訓���練���範式，使語音模型專注於真實音���訊理解而非上下文猜���測，降低���錯���誤���傳播風���險。

## 補充細節

方法：AGSC ��� � � 包含三步���驟：從音���訊合成含答案的線索、���篩選直接暴���露答案與音���訊依���賴的線索、作為可移除���訓���練���腳架使用。GDPO ��� � � 階段學���習聯���鎖���閘門-plus-���轉錄���輸出用於���串流控制。實���驗：在重���疊+���噪音、會議、���串流語音情境上���驗���證；無線索平均 mpWER 下降幅度達 68%–79%。程式���碼、manifests、���證據與公開語音食���譜隨論文���釋出。

## 維護紀錄

- 收錄日期：2026-08-10
- 最後更新：2026-08-10

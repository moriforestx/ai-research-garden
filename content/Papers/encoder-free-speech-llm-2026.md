---
title: "LLM Can Read Spectrogram: Encoder-Free Speech-Language Modeling"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-10"
organization: "作者未明（來自 arXiv）"
source_url: "https://arxiv.org/abs/2606.10231"
date_collected: "2026-09-12"
date_updated: "2026-09-12"
tags:
  - ai
  - paper
---

# LLM Can Read Spectrogram: Encoder-Free Speech-Language Modeling

## 基本資訊

- 發布日期：2026-06-10
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2606.10231

## 概要

本研究提出 Mel-LLM，一種編碼器自由的語音語言模型架構，移除傳統的預訓練語音編碼器（特別是 Transformer/Conformer 區塊），仅保留用於下採樣的卷積層。Mel 頻譜圖在時間維度被分塊，並透過線性投射直接映射到 LLM 的嵌入空間。LLM 自身學習解讀這些原始頻譜特徵並與文字對齊，僅使用其自身的 Transformer 層。實驗顯示，編碼器自由方法在自動語音識別（ASR）上達到與編碼器初始化模型相近的效能，尤其是在訓練資料充足時。Phi‑4-MM 初始化在低資源環境中關鍵。消融研究發現較低的 LLM 層對隱式語音編碼最為重要。

## 核心價值

直接將 Mel 頻譜圖投射至 LLM 的編碼器自由語音語言模型

## 應用情境與實務影響

簡化語音與文字建模管線，降低模型複雜度與延遲，使語音理解系統在資源受限設備上更易部署。

## 補充細節

論文提供了 Encoder‑free vs Encoder‑based 的詳細比較，涵蓋多個資料規模。模型使用輕度預處理的 Mel 頻譜圖塊，透過線性投射入 LLM。在低資源情境下，Phi‑4-MM 初始化顯著提升效能。

## 維護紀錄

- 收錄日期：2026-09-12
- 最後更新：2026-09-12

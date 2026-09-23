---
title: "SwanTale: Unified Multi-Speaker Speech and Audio Generation for Instruct and Zero-Shot Tasks"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-08-25"
organization: "arXiv"
source_url: "https://arxiv.org/html/2608.02023v2"
date_collected: "2026-09-24"
date_updated: "2026-09-24"
tags:
  - ai
  - paper
---

# SwanTale: Unified Multi-Speaker Speech and Audio Generation for Instruct and Zero-Shot Tasks

## 基本資訊

- 發布日期：2026-08-25
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/html/2608.02023v2

## 概要

提出 SwanTale，一個統一的多說話者語音與音訊生成模型，支援指令跟隨（instruct）和零樣本（zero-shot）任務。透過 SwanVAE（流動 Transformer）、Engram 條件式編碼、統一混合專家（Unified MoE）等架構創新，實現從自然語言描述設計說話者聲音、透過參考音訊重複使用聲音，以及在單一波形中聯合生成語音、環境音與局部音訊效果。模型同時支援語音內容編輯、說話者身份轉換與情感控制。

## 核心價值

首次實現端到端統一的語音與音訊生成框架，將說話者身份控制、環境音合成與語音編輯整合於單一模型中，顯著降低複雜音訊生成管線的模組數量與遲延。

## 應用情境與實務影響

適用於虛擬助理、有聲書製作、遊戲聲音設計、雙語 doppiage 等場景；支援零樣本聲音克隆與跨語言語音轉換；降低聲音製作的專業門檻與成本。

## 補充細節

論文於 2026-08-02 初次提交，2026-08-25 更新 v2 版本。SwanTale 架構包括：(1) SwanVAE：基於流動 Transformer 的變分自編碼器，具獎勵條件品質控制；(2) Engram 條件式編碼：從參考音訊中提取說話者特徵；(3) Unified MoE：統一混合專家層，平衡指令遵循與聲音品質；(4) 透過 curriculum learning 與 GRPO（Generative Reward Policy Optimisation）後訓練對齊人類偏好。SwanData-Caption 提供監督訊號，包含目標資料覆蓋、語音相前處理、多級標註與品質過濾。模型能從自然語言如「製造一個帶有輕微蘇格蘭口音的年長女性聲音」生成對應聲音；透過 5 秒參考音訊重現特定說話者的聲學特徵；在單一波形中同時生成對話語音、背景雨聲與腳步聲。在語音生成基準上，SwanTale 在 MOS（Mean Opinion Score）達到 4.4/5.0，聲音相似度（Speaker Encoder Cosine）達到 0.87，顯著優於之前的分階段管線方法。

## 維護紀錄

- 收錄日期：2026-09-24
- 最後更新：2026-09-24

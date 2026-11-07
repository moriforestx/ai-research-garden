---
title: "Qwen-Audio-3.0-TTS: Freely Controllable and Highly Robust Speech Synthesis with Multi-Stage Training Paradigm"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-07-27"
organization: "Alibaba Cloud (Qwen Team)"
source_url: "https://arxiv.org/abs/2607.23938"
date_collected: "2026-11-08"
date_updated: "2026-11-08"
tags:
  - ai
  - paper
---

# Qwen-Audio-3.0-TTS: Freely Controllable and Highly Robust Speech Synthesis with Multi-Stage Training Paradigm

## 基本資訊

- 發布日期：2026-07-27
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2607.23938

## 概要

阿里巴巴 Qwen 團隊提出 Qwen-Audio-3.0-TTS，採用五階段訓練範式（步驟 ③-⑤ 專門「消除弱點」），實現單一模型整合多語言/多方言合成、零樣本語音克隆、自由風格指令跟隨、細粒度內聯控制、單通道長文本生成與抗退化提示魯棒性。在 2026/07/16 Artificial Analysis TTS Arena 盲測中，Qwen-Audio-3.0-TTS-Plus 以 Elo 1237 奪冠，跨 16 語言平均講者相似度 82.75 領先同類。

## 核心價值

首個在獨立第三方排行榜奪冠的開放權重級 TTS 模型，以多階段「消除弱點」訓練解決長文本、指令跟隨、真實環境雜訊等痛點。

## 應用情境與實務影響

適用於多語言客服語音、有聲書長文本生成、即時語音翻譯、語音克隆輔助工具、方言保存與教學。論文提供可擴展的講者適配協議，降低工業界部署門檻。

## 補充細節

論文編號 arXiv:2607.23938v1，分類 eess.AS。提交日期 2026-07-27。核心創新：五階段訓練管線（預訓練→指令微調→弱點消除×3），統一架構支援 16+ 語言與多種中文方言。官方部落格 (alibabacloud.com) 提供詳細基準數據。代碼與模型權重預期開源於 QwenLM 組織。

## 維護紀錄

- 收錄日期：2026-11-08
- 最後更新：2026-11-08

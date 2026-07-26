---
title: "An Efficient vLLM-Based Inference Pipeline for Unified Audio Understanding and Generation"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-07-02"
organization: "Tokyo University of Science / Carnegie Mellon University"
source_url: "https://arxiv.org/abs/2607.02119"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - paper
---

# An Efficient vLLM-Based Inference Pipeline for Unified Audio Understanding and Generation

## 基本資訊

- 發布日期：2026-07-02
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2607.02119

## 概要

Watanabe 團隊於 2026 年 7 月 2 日發表 arXiv:2607.02119，提出基於 vLLM 推理引擎的統一音訊理解與生成管線。針對語音語言模型（SLM）採用解耦 AR+NAR 或延遲模式交錯的 Multi-Token Prediction (MTP) 生成多層音訊 token，與標準單流解碼循環衝突，導致高吞吐引擎難以原生支援多模態生成。本文在 vLLM 中擴展自迴歸解碼，原生執行 delay-pattern de-interleaving 與協調多流採樣，並整合 GPU 上的聲學解碼器實現端到端波形合成。關鍵創新在於 Classifier-Free Guidance (CFG) 並行排程：將條件與無條件請求配對放入連續批次，吸收雙請求與 logit 合併開銷，使 CFG 吞吐量維持非 CFG 的 80% 以上。框架已開源。

## 核心價值

首個在 vLLM 上原生支援語音理解與生成的高吞吐推理管線，解決 CFG 吞吐量折半的長期痛點，為大規模部署語音 LLM 提供關鍵工程基礎設施。

## 應用情境與實務影響

語音 LLM 服務提供商可直接整合此管線實現低延遲、高並發的端到端語音對話系統；開源社群可基於此框架快速構建統一理解/生成的多模態音訊應用，降低部署門檻。

## 補充細節

作者：Haoran Wang、Jinchuan Tian、Siddhant Arora、Shinji Watanabe（東京科學大學 / Carnegie Mellon University）。提交日期 2026-07-02。實驗於 A100/H100 GPU 驗證，支援 LLaMA-Omni、SpeechGPT 等主流 SLM 架構。代碼已發布於 GitHub。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

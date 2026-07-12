---
title: "OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-04-01"
authors: []
keywords: []
identifier: "2604.00688"
identifier_type: "arXiv"
publication_status: "preprint"
source_url: "https://arxiv.org/html/2604.00688v3"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# OmniVoice: Towards Omnilingual Zero-Shot Text-to-Speech with Diffusion Language Models

## 基本資訊

- 作者：k2-fsa 研究團隊
- 發布日期：2026-04-01
- 研究主題：音訊與語音 / Audio & Speech
- 關鍵字：零樣本語音合成、多語言 TTS、擴散語言模型、聲碼本
- 論文識別碼：2604.00688 (arXiv)
- 發表狀態：預印本
- 主要來源：https://arxiv.org/html/2604.00688v3

## 摘要

OmniVoice 實現大規模多語言零樣本 TTS，支援 600 種以上語言。採用擴散語言模型將文本直接映射到多聲碼本聲學 Token，結合全聲碼本隨機遮蔽與 LLM 初始化，使用 581k 小時開源數據訓練，在中文、英文及多語言基準上達到 SOTA。

## 核心研究問題

如何在無需針對每種語言單獨訓練的情況下，實現高品質的多語言零樣本語音合成？

## 方法與技術

擴散語言模型架構，文本到多聲碼本聲學 Token 的直接建模，全聲碼本隨機遮蔽訓練策略，利用預訓練 LLM 初始化加速收斂。

## 實驗與研究結果

在中文、英文及多語言 TTS 基準上達到最優表現，支援 600+ 語言零樣本合成。

## 研究意義與適用範圍

大幅降低多語言 TTS 部署門檻，適用於多語言語音助手、無障礙工具、跨語言內容生成等場景。

## 限制與注意事項

低資源語言合成品質有待提升；推理延遲較傳統 TTS 系統高。

## 相關概念

- 零樣本語音合成
- 擴散模型
- 多語言 TTS
- 聲碼本建模

## 相關工具與專案

- OmniVoice 實作：https://github.com/k2-fsa/OmniVoice

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

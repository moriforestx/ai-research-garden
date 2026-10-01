---
title: "ExaServe: Large-Scale LLM Serving on Exascale HPC Systems"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-11"
organization: "University of Chicago / Argonne National Laboratory"
source_url: "https://arxiv.org/abs/2609.10812"
date_collected: "2026-10-02"
date_updated: "2026-10-02"
tags:
  - ai
  - paper
---

# ExaServe: Large-Scale LLM Serving on Exascale HPC Systems

## 基本資訊

- 發布日期：2026-09-11
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2609.10812

## 概要

本文提出 ExaServe，一個在批次排程 HPC 系統上部署 Ray Serve LLM 推理的可復現框架，於 ALCF Aurora 超算（Intel XPU）從 1 到 256 節點（3072 vLLM 複本）開發與評測。非串流推理吞吐近線性擴展：單一 head-node HAProxy 在 256 節點達 27.1k QPS（3.8M tokens/s），與直接派送基準持平；串流模式在互動 SLO 下於中等節點數即達標。論文詳細刻畫兩種擴展機制，並開源部署腳本與效能分析工具。

## 核心價值

首個在百萬級 token/s 規模驗證 Ray Serve + vLLM/SGLang 在 exascale HPC 上的近線性擴展，提供開箱即用的部署範式與效能基準。

## 應用情境與實務影響

為科學計算工作流（文獻挖掘、實驗導向代理、評估器在環訓練）引入 LLM 推理提供可直接落地的 HPC 部署方案；對雲端/混合雲大模型服務架構設計具參考價值。

## 補充細節

arXiv:2609.10812v2 [cs.DC]，提交日期 2026-09-11（v1 為 2026-09-10）。作者：Wenyi Wang、Shu Shi、Yadu Babuji、Ian Foster、Kyle Chard（芝加哥大學 / 阿貢國家實驗室）。涵蓋 MPI、Ray Serve、vLLM、SGLang、Intel XPU、Aurora 超算。

## 維護紀錄

- 收錄日期：2026-10-02
- 最後更新：2026-10-02

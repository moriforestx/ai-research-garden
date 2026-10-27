---
title: "RayRoPE: Projective Ray Positional Encoding for Multi-view Attention"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-08"
organization: "Carnegie Mellon University, Apple"
source_url: "https://eccv.ecva.net/virtual/2026/poster/4570"
date_collected: "2026-10-28"
date_updated: "2026-10-28"
tags:
  - ai
  - paper
---

# RayRoPE: Projective Ray Positional Encoding for Multi-view Attention

## 基本資訊

- 發布日期：2026-09-08
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://eccv.ecva.net/virtual/2026/poster/4570

## 概要

ECCV 2026 Spotlight 論文，提出 RayRoPE 位置編碼機制，專為多視角 Transformer 設計，透過光線投影座標實現 SE(3) 不變性注意力。作者來自 CMU 與 Apple，針對多視角注意力中現有絕對/相對位置編碼無法同時滿足幾何唯一性、SE(3) 不變性與場景自適應三大需求的缺口，給出理論完備且實證優於基線的解法。

## 核心價值

為多視角視覺 Transformer 確立了幾何感知位置編碼新標準，代碼與權重已開源，可直接整合至 3D 重建、新穎視角合成與具身 AI 管線。

## 應用情境與實務影響

提升多視角注意力在大規模場景、長序列下的幾何一致性與推理效率；對自動駕駛感知、機器人導航、大規模 3D 高斯濃縮渲染等下游任務具直接遷移價值。

## 補充細節

ECCV 2026 於 2026-09-08 至 09-12 在瑞典馬爾默舉辦，該論文獲選為 Spotlight（口頭報告比例約 2.5%）。arXiv 預印本：2601.15275v1；官方專案頁：https://rayrope.github.io；代碼倉庫：https://github.com/Lucas-707/RayRoPE (MIT License)；Apple ML 研究部落格同步發布：https://machinelearning.apple.com/research/rayrope-projective-ray。作者：Yu Wu、Minsik Jeon (CMU)、Jen-Hao Rick Chang、Oncel Tuzel (Apple)、Shubham Tulsiani (CMU)。

## 維護紀錄

- 收錄日期：2026-10-28
- 最後更新：2026-10-28

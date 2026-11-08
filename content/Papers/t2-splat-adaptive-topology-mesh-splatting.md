---
title: "T²-Splat: 具適應拓樸的網格濺射技術結合紋理殘差"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-11-06"
organization: "NeurIPS 2026"
source_url: "https://arxiv.org/abs/2611.06974"
date_collected: "2026-11-09"
date_updated: "2026-11-09"
tags:
  - ai
  - paper
---

# T²-Splat: 具適應拓樸的網格濺射技術結合紋理殘差

## 基本資訊

- 發布日期：2026-11-06
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2611.06974

## 概要

論文提出 T²-Splat，將拓樸適應與外觀精煉解耦：先用安全限制德洛內三角剖分初始化網格連接，再透過動態拓樸演化調整三角形分配，最後以殘差逐面 Mip-map 紋理精煉外觀。在 Mip-NeRF 360、Tanks & Temples、DTU 基準測試上表現優異，PSNR 比 MeshSplatting 高 0.71dB，且支援將面數壓縮至原本的 10%。已獲 NeurIPS 2026 接收。

## 核心價值

三角形濺射技術突破，以拓樸與外觀分離設計實現高品質新視角合成並大幅降低幾何複雜度。

## 應用情境與實務影響

為 3D 高斯濺射與傳統網格渲染管線整合提供實用路徑，適用於即時渲染、壓縮傳輸與跨平台部署場景。

## 補充細節

作者：Zhihao Tang、Youjia Zhang、Mingbo Zhao、Wei Yang。專案頁面：https://t2-splat.github.io/。論文編號 arXiv:2611.06974v1，提交於 2026-11-06。屬 cs.CV、cs.GR 分類。

## 維護紀錄

- 收錄日期：2026-11-09
- 最後更新：2026-11-09

---
title: "Apple researchers introduce Drop-In Perceptual Optimization for 3D Gaussian Splatting accepted to ECCV 2026"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-15"
organization: "Apple"
source_url: "https://machinelearning.apple.com/updates/apple-at-eccv-2026"
date_collected: "2026-09-04"
date_updated: "2026-09-04"
tags:
  - ai
  - paper
---

# Apple researchers introduce Drop-In Perceptual Optimization for 3D Gaussian Splatting accepted to ECCV 2026

## 基本資訊

- 發布日期：2026-07-15
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://machinelearning.apple.com/updates/apple-at-eccv-2026

## 概要

Apple 研究團隊提出一種名為 Drop-In Perceptual Optimization 的新方法，可直接改進 3D 高斯溶聚（3D Gaussian Splatting）技術，使其在保持原始架構不變的情況下，透過感知導向的優化顯著提升渲染品質與效率，特別是在複雜光照和材質場景中表現尤為突出。

## 核心價值

無需修改現有 3D 高斯溶聚管線即可插入的感知品質優化方法。

## 應用情境與實務影響

該方法可直接應用於擴增實境、虛擬實境、數位 twin 及內容創作等領域，提升 3D 內容的視覺真實感與渲染效能，降低存儲與計算需求。

## 補充細節

論文由 Ezgi Ozyilkan、Zhiqi Chen、Oren Rippel、Jona Ballé（紐約大學）和 Kedar Tatwawadi 共同撰寫，論文編號 #129，已被歐洲計算機視覺會議（ECCV 2026）接收。方法透過在渲染過程中引入感知損失函數，優化高斯點的位置、協方差和顏色屬性，使生成的 3D 場景在保持幾何準確性的同時，更符合人類視覺系統對光照、反射和材質的感知特徵。實驗顯示在多個基準測試中相比原始方法達到最高 37% 的 PSNR 提升和 22% 的渲染速度提升。

## 維護紀錄

- 收錄日期：2026-09-04
- 最後更新：2026-09-04

---
title: "URVIS 2026: Adverse-to-Extreme Panoptic Segmentation Challenge"
type: paper
research_topic: "電腦視覺 / Computer Vision"
date_published: "2026-04-18"
date_collected: "2026-07-14"
date_updated: "2026-07-14"
source_url: "https://arxiv.org/abs/2604.16984"
identifier: "urvis-2026-cvpr-both-2026"
tags:
  - ai
  - paper
  - computer-vision
  - panoptic-segmentation
  - multimodal-perception
  - adverse-weather
---

# URVIS 2026: Adverse-to-Extreme Panoptic Segmentation Challenge

## 概述

URVIS 2026 是針對惡劣至極端天候環境所設計的多模態全景分割挑戰。研究使用 MUSES 多感測器資料集，整合 RGB 相機、LiDAR、雷達與事件相機資料，評估模型在霧、雨、雪、夜間與其他低能見度條件下的場景理解能力。

本報告整理挑戰設定、參賽方法、基準結果與現階段仍待解決的問題，核心目標是提升自動駕駛與機器人在困難環境中的感知魯棒性。

## 研究設定

- **任務**：惡劣至極端天候下的全景分割
- **資料集**：MUSES
- **感測器模態**：
  - RGB 相機
  - LiDAR
  - 雷達
  - 事件相機
- **主要評估指標**：Weighted Panoptic Quality（wPQ）
- **參與規模**：
  - 17 位註冊參與者
  - 47 次提交
  - 4 組團隊進入最終階段

## 核心貢獻

1. 建立首個聚焦惡劣至極端環境的全景分割挑戰與比較基準。
2. 使用多感測器資料評估不同模態在低能見度與複雜天候下的互補效果。
3. 提出 Weighted Panoptic Quality，降低不同天候條件分布不均對整體排名造成的偏差。
4. 系統整理參賽方法的設計、效能與失敗模式。
5. 指出目前多模態全景分割在感測器融合、跨天候泛化與極端條件穩定性方面仍有明顯改善空間。

## 核心價值

一般視覺模型多在正常光照與良好天候條件下訓練與測試，實際部署至自動駕駛、道路監控或戶外機器人時，容易因霧、雨、雪、夜間與感測器退化而失效。

URVIS 2026 提供更接近真實部署風險的評估環境，讓研究者能比較不同感測器組合與融合方法在極端條件下的可靠性。

## 應用情境與實務影響

- 自動駕駛車輛的全天候場景理解
- 戶外機器人在低能見度環境中的導航
- 道路與交通監控
- 搜救與災害應變系統
- 多感測器融合模型的魯棒性測試
- 感知系統部署前的極端條件驗證

## 限制與待觀察事項

- 挑戰結果主要反映 MUSES 資料分布，未必能直接代表所有地區與感測器配置。
- 多感測器融合會增加硬體成本、同步複雜度與推論負擔。
- 極端天候樣本仍相對有限，跨地區與跨設備泛化能力需要進一步驗證。
- wPQ 能改善不同天候條件的評估公平性，但仍不能完全涵蓋安全關鍵失敗模式。

## 來源

- 原始論文：https://arxiv.org/abs/2604.16984
- URVIS 挑戰網站：https://urvis-workshop.github.io/challenge-Muses.html

---
title: "NitroGen：面向泛用遊戲代理人的開放基礎模型"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-01"
organization: "NVIDIA"
source_url: "https://research.nvidia.com/labs/lpr/publication/magne2026nitrogenopenfoundationmodel"
date_collected: "2026-11-22"
date_updated: "2026-11-22"
tags:
  - ai
  - paper
---

# NitroGen：面向泛用遊戲代理人的開放基礎模型

## 基本資訊

- 發布日期：2026-06-01
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://research.nvidia.com/labs/lpr/publication/magne2026nitrogenopenfoundationmodel

## 概要

NVIDIA 研究團隊發表 NitroGen，首個面向泛用遊戲代理人的開放視覺-動作基礎模型。模型在超過 1,000 款遊戲、40,000 小時遊玩影片上以大規模行為克隆訓練，輸入原始 RGB 影格即可輸出手把動作。架構採用流匹配生成動作塊，視覺骨幹為 SigLIP 2 ViT，於 CVPR 2026 以 Oral 發表。模型權重、資料集與基準環境皆已開源釋出。

## 核心價值

首個跨遊戲泛化的視覺-動作基礎模型，證明純視覺輸入即可實現零樣本跨遊戲控制，為具身智慧與通用代理人研究提供重要基座。

## 應用情境與實務影響

開源模型與資料集降低遊戲 AI 研究門檻；流匹配動作生成機制可遷移至機器人控制與模擬環境；多遊戲基準環境推動跨任務泛化評測標準化。

## 補充細節

論文編號 arXiv:2601.02427，CVPR 2026 Oral。訓練資料透過自動化關鍵點匹配（SIFT/XFeat）從公開遊玩影片提取手把動作標註，構建網際網路規模視頻-動作資料集。模型在未見遊戲上達 40-60% 成功率，3D 遊戲表現優於 2D。Hugging Face 託管模型權重（nvidia/NitroGen），專案官網 nitrogen.minedojo.org 提供互動 Demo 與 Gymnasium 環境包裝器。

## 維護紀錄

- 收錄日期：2026-11-22
- 最後更新：2026-11-22

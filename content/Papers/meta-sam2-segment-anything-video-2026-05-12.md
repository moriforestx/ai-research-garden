---
title: "SAM 2: Segment Anything in Images and Videos"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-05-12"
organization: "Meta AI"
source_url: "https://ai.meta.com/research/publications/sam-2-segment-anything-in-images-and-videos"
date_collected: "2026-08-10"
date_updated: "2026-08-10"
tags:
  - ai
  - paper
---

# SAM 2: Segment Anything in Images and Videos

## 基本資訊

- 發布日期：2026-05-12
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://ai.meta.com/research/publications/sam-2-segment-anything-in-images-and-videos

## 概要

Meta AI 於 2026 年 5 月 12 日發布 SAM 2，首個統一的�圖像與視�頻分割基�礎模型。�繼承 SAM 的提示式設計，新增逐會話記�憶模組，可在視�頻中追��蹤物件、處理�遮�擋與重現，支援即時�串流推理。在 17 � 個視�頻分割基準與 37 � 個�圖像分割資料集上達到 SOTA，零�樣本�泛化能力強。

## 核心價值

將提示式分割從�靜態�圖像�擴展到視�頻域，單一模型統一處理�圖像/視�頻分割與追��蹤，開源權重與程式�碼，大幅降低視�覺應用開發門�檻。

## 應用情境與實務影響

適用於視�頻編輯、自動�駕�駛感知、機器人視�覺、�醫�療影像分�析、AR/VR 物件追��蹤等需長時序一致分割的場景；記�憶機制設計可移�植至其他視�頻理解任務。

## 補充細節

架構：ViT-H 影像編�碼器 + �� 輕量�掩碼解�碼器 + 記�憶注意力模組（�儲存每�幀物件��嵌入，�跨�幀注意力查�詢）。�訓�練資料：SA-V � 資料集（51k 視�頻、600k+ � 掩�碼標註），比 SA-1B 大 4.5 � 倍。效能：A100 上 44 FPS 即時推理。開源：Apache 2.0 � 授權，權重與程式�碼於 GitHub 發布。論文：arXiv:2408.00714v2。作者：Nikhila Ravi 等 22 人。

## 維護紀錄

- 收錄日期：2026-08-10
- 最後更新：2026-08-10

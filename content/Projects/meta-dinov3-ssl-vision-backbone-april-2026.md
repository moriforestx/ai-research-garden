---
title: "Meta 發布 DINOv3：自監督學習規模化新里程碑的通用視覺骨幹"
type: project
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-04-08"
organization: "Meta AI"
source_url: "https://ai.meta.com/blog/dinov3-self-supervised-vision-model"
date_collected: "2026-08-25"
date_updated: "2026-08-25"
tags:
  - ai
  - project
---

# Meta 發布 DINOv3：自監督學習規模化新里程碑的通用視覺骨幹

## 基本資訊

- 發布日期：2026-04-08
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://ai.meta.com/blog/dinov3-self-supervised-vision-model

## 概要

Meta AI 於 2026 年 4 月 8 日發布 DINOv3，將自監督學習 (SSL) 規模擴大至 17 億張圖像與 70 億參數，首次讓單一凍結視覺骨幹在物件偵測、語義分割等密集預測任務上超越專用模型。釋出含 ViT 與 ConvNeXt 變體的完整模型套件，含衛星影像專用骨幹，採商業授權開放。

## 核心價值

以大規模 SSL 產出通用高解析度視覺特徵，單一骨幹即可跨領域達 SOTA，簡化下游任務適配流程。

## 應用情境與實務影響

研究者與開發者可直接使用凍結骨幹進行零樣本或微調部署，涵蓋衛星測圖、機器人視覺、深度估計等場景；提供筆記本與評測頭複現基準。

## 補充細節

官方部落格宣稱 DINOv3 為 SSL 規模化新里程碑：模型大小較 v2 擴大 6 倍、訓練資料擴大 12 倍。引入 Gram anchoring 技術實現超銳利特徵（支援 4096×4096 解析度）。同步釋出 Hugging Face 模型卡、GitHub 代碼與推理筆記本。商業授權允許生產環境使用。Roboflow 於 4/8 發佈訓練指南確認釋出時間。

## 維護紀錄

- 收錄日期：2026-08-25
- 最後更新：2026-08-25

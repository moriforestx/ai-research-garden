---
title: "SAM Audio：首個統一多模態音訊分離模型"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-11-12"
organization: "Meta AI (FAIR)"
source_url: "https://ai.meta.com/blog/sam-audio"
date_collected: "2026-11-20"
date_updated: "2026-11-20"
tags:
  - ai
  - tool
---

# SAM Audio：首個統一多模態音訊分離模型

## 基本資訊

- 發布日期：2026-11-12
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://ai.meta.com/blog/sam-audio

## 概要

Meta AI 於 2026 年 11 月 12 日發布 SAM Audio，首個統一多模態模型，可從複雜音訊混合中使用自然語言、視覺線索或時間區段提示隔離任意聲音。基於流匹配擴散 Transformer 架構，支援文字提示（如「狗叫聲」）、視覺提示（點擊視頻物件提取對應聲音）與區段提示（標記目標聲音出現的時間段）。同步開源 PE-AV（Perception Encoder Audiovisual）、SAM Audio-Bench（首個實況音訊分離基準）與 SAM Audio Judge（首個自動評分模型）。模型訓練於超 1 億影片的大規模多模態對比學習數據。

## 核心價值

將 Segment Anything 的提示式分割範式延伸至音訊領域，實現零樣本、多模態提示驅動的通用聲音分離。

## 應用情境與實務影響

音樂製作、播客後製、影視配音、無障礙工具等場景可透過 Segment Anything Playground 直接體驗，大幅降低音訊編輯門檻；研究者獲得首個統一基準與評分模型推動領域發展。

## 補充細節

架構採用流匹配擴散 Transformer，處理音訊混合與提示生成分離音軌。訓練數據涵蓋語音、音樂、聲音事件的真實與合成混合。已知限制：不支援音訊提示、無法無提示完整分離、對相似聲音事件（如合唱團個別人聲）分離效果較弱。代碼、權重與論文開源。

## 維護紀錄

- 收錄日期：2026-11-20
- 最後更新：2026-11-20

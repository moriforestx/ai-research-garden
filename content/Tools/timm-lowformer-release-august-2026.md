---
title: "timm 釋出 LowFormer 模型權重，提供硬體效率優化的視覺骨幹架構"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-08-27"
organization: "Hugging Face / Altair199797 (LowFormer 作者)"
source_url: "https://github.com/huggingface/pytorch-image-models/releases/tag/1.0.29"
date_collected: "2026-09-21"
date_updated: "2026-09-21"
tags:
  - ai
  - tool
---

# timm 釋出 LowFormer 模型權重，提供硬體效率優化的視覺骨幹架構

## 基本資訊

- 發布日期：2026-08-27
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://github.com/huggingface/pytorch-image-models/releases/tag/1.0.29

## 概要

PyTorch Image Models (timm) 釋出 1.0.29 版本，新增 LowFormer 模型與預訓練權重。LowFormer 是針對硬體效率優化的視覺骨幹架構家族，包含 Lowtention（輕量化多頭自注意力替代方案），在 GPU、Jetson TX2 與 ARM CPU 上達到最佳速度-精度權衡。提供基礎模型 B0-B3 及邊緣 GPU 變體 E1/E2/E3，適合邊緣部署場景。

## 核心價值

將學術提出的硬體感知架構（IJCV 2026 期刊論文）轉化為可直接在 timm 中使用的預訓練模型，降低開發者在邊緣裝置部署高效視覺骨幹的門檻。

## 應用情境與實務影響

開發者可直接從 timm 載入 LowFormer 預訓練權重進行微調或推理，無需自行實作複雜的 Lowtention 注意力機制；邊緣部署場景（機器人、移動裝置、IoT）可受益於其在 Jetson TX2 與 ARM CPU 上的優異延遲表現。

## 補充細節

LowFormer 最初於 WACV 2025 發表，延伸版於 2026 年刊載於 International Journal of Computer Vision (doi:10.1007/s11263-026-02873-5)。架構特色：宏觀設計簡化階段數與下採樣策略，微觀設計引入 Lowtention 取代 MHSA，大幅降低記憶體存取與計算開銷。timm 1.0.29 同步修正多項由代理人發現的細微錯誤。來源：Hugging Face pytorch-image-models 官方倉庫與 PyPI 釋出紀錄。

## 維護紀錄

- 收錄日期：2026-09-21
- 最後更新：2026-09-21

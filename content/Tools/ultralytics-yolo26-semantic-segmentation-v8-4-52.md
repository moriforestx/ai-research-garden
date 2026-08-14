---
title: "Ultralytics YOLO26 新增原生語意分割支援 (v8.4.52)"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-05-20"
organization: "Ultralytics"
source_url: "https://community.ultralytics.com/t/new-release-ultralytics-v8-4-52/1981"
date_collected: "2026-08-14"
date_updated: "2026-08-14"
tags:
  - ai
  - tool
---

# Ultralytics YOLO26 新增原生語意分割支援 (v8.4.52)

## 基本資訊

- 發布日期：2026-05-20
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://community.ultralytics.com/t/new-release-ultralytics-v8-4-52/1981

## 概要

Ultralytics 釋出 v8.4.52 版本，為 YOLO26 帶來原生語意分割作為一級任務支援。新增預訓練 `-sem` 模型、端到端訓練與推論支援、匯出相容性、更廣泛資料集支援與更強測試覆蓋。訓練增強功能現支援語意遮罩，語意分割模型在匯出與部署流程中運作更順暢。

## 核心價值

將即時物件偵測框架 YOLO26 擴展為完整的語意分割解決方案，單一模型族群涵蓋偵測、分割、姿態、分類、OBB 多任務，大幅簡化邊緣部署與多任務管線。

## 應用情境與實務影響

開發者可用單一 YOLO26 模型完成像素級場景理解，無需切換專用分割架構；邊緣裝置部署受益於 NMS-free、DFL 移除的精簡架構；支援 ONNX、OpenVINO、TensorRT 等主流匯出格式。

## 補充細節

v8.4.52 釋出於 2026-05-20。核心更新：語意分割原生支援（`-sem` 模型）、增強功能遮罩處理、匯出部署優化。配合 v8.4.0 (2026-01-14) 引入的 YOLO26 核心架構：端到端無 NMS 推論、MuSGD 混合優化器、移除 DFL、YOLOE-26 開放詞彙偵測。官方文件：https://docs.ultralytics.com

## 維護紀錄

- 收錄日期：2026-08-14
- 最後更新：2026-08-14

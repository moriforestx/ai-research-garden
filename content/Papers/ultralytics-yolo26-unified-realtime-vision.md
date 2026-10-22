---
title: "Ultralytics YOLO26：統一即時端到端視覺模型"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-06-02"
organization: "Ultralytics"
source_url: "https://arxiv.org/abs/2606.03748"
date_collected: "2026-10-23"
date_updated: "2026-10-23"
tags:
  - ai
  - paper
---

# Ultralytics YOLO26：統一即時端到端視覺模型

## 基本資訊

- 發布日期：2026-06-02
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2606.03748

## 概要

Ultralytics 發表 YOLO26，一個統一的即時視覺模型家族，解決現有 YOLO 檢測器依賴 NMS、檢測頭較重、訓練週期長、小物件正樣本覆蓋不足等問題。YOLO26 採用雙頭設計實現原生 NMS-free 端到端推理，完全移除 DFL，並引入 MuSGD 混合優化器、Progressive Loss 訓練策略與 STAL 標籤分配策略。模型家族涵蓋五種規模（n/s/m/l/x），支援檢測、實例分割、姿態估計、分類與定向檢測，並在 COCO 上達到 40.9-57.5 mAP、T4 TensorRT 延遲 1.7-11.8 ms。

## 核心價值

首個在單一管線中統一檢測、分割、姿態、分類與定向檢測並達 SOTA 即時效能的開源模型家族；NMS-free 端到端推理大幅簡化部署複雜度。

## 應用情境與實務影響

邊緣裝置與生產環境可直接部署單一模型處理多種視覺任務，減少模型維護成本；NMS-free 架構降低推理延遲並簡化 ONNX/TensorRT/ CoreML 導出流程。

## 補充細節

論文 31 頁、8 圖；程式碼與模型開源於 https://github.com/ultralytics/ultralytics。同期發布開放詞彙擴展 YOLOE-26，支援文字、視覺與無提示推理。

## 維護紀錄

- 收錄日期：2026-10-23
- 最後更新：2026-10-23

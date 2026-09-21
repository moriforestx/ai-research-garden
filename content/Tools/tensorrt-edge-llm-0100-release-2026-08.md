---
title: "TensorRT Edge-LLM 0.10.0：支援 Nemotron-3.5 系列與 ONNX-less 引擎建構"
type: tool
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-08-15"
organization: "NVIDIA"
source_url: "https://github.com/nvidia/tensorrt-edge-llm"
date_collected: "2026-09-22"
date_updated: "2026-09-22"
tags:
  - ai
  - tool
---

# TensorRT Edge-LLM 0.10.0：支援 Nemotron-3.5 系列與 ONNX-less 引擎建構

## 基本資訊

- 發布日期：2026-08-15
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://github.com/nvidia/tensorrt-edge-llm

## 概要

NVIDIA 於 2026 年 8 月發布 TensorRT Edge-LLM 0.10.0，新增對 Nemotron-3.5 Lightning (MTP/DFlash)、Cosmos3-Edge、DiffusionGemma、Nemotron-3.5-ASR 及 DSpark 推測解碼的 Day-0 支援。關鍵創新包含實驗性 ONNX-less 直接 TensorRT 引擎建構器、多輪 KV-cache 重用、實驗性 OpenAI 相容服務器支援視頻輸入。同期 0.10.1 (9 月) 推出雙 DGX Spark TP=2 推理與服務器冷啟動優化。框架專為 DRIVE AGX Thor 與 Jetson Thor 等嵌入式物理 AI 平台設計，C++ 純運行時無 Python 依賴。

## 核心價值

邊緣 LLM/VLM 推理框架首次實現免 ONNX 導出的直接引擎建構，配合多輪 KV-cache 重用大幅降低對話延遲，Nemotron-3.5 系列 Day-0 支援縮短新模型上車週期。

## 應用情境與實務影響

汽車/機器人開發者可跳過 ONNX 轉換步驟直建引擎，多輪對話場景受益於 KV-cache 重用；Nemotron-3.5-ASR 整合語音理解，Cosmos3-Edge 支援世界模型推理，擴展 Physical AI 應用邊界。

## 補充細節

架構：C++ 輕量運行時、優化 CUDA Kernel、FP8/INT4/NVFP4 量化、EAGLE-3/DSpark/DDTree 推測解碼。模型支援擴展至 Gemma 4 全系、Qwen3-Omni、Qwen3.8-27B、Nemotron-3 NVFP4。文檔站: nvidia.github.io/TensorRT-Edge-LLM/latest。GitHub: nvidia/tensorrt-edge-llm (Apache-2.0)。

## 維護紀錄

- 收錄日期：2026-09-22
- 最後更新：2026-09-22

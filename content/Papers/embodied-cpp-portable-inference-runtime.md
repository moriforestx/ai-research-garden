---
title: "Embodied.cpp：異構機器人上具身 AI 模型的可移植推理運行時"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-03"
organization: "SEU-PAISys / Technology Innovation Institute (TII)"
source_url: "https://arxiv.org/abs/2607.02501"
date_collected: "2026-08-15"
date_updated: "2026-08-15"
tags:
  - ai
  - paper
---

# Embodied.cpp：異構機器人上具身 AI 模型的可移植推理運行時

## 基本資訊

- 發布日期：2026-07-03
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2607.02501

## 概要

來自 SEU-PAISys 與 TII 的研究團隊發布 Embodied.cpp，一個面向 Vision-Language-Action (VLA) 與 World-Action Models (WAM) 的輕量級 C++ 推理運行時。透過五層模組化架構（輸入適配器、序列構建器、骨幹執行、頭部插件、部署適配器），支援 CPU/CUDA GPU/NPU 異構硬體上的批次大小 1 高效推理，模型權重採用 GGUF 格式，記憶體佔用從 200+ MiB 壓縮至 88 MiB，並開源於 GitHub (Apache 2.0)。

## 核心價值

首個專為具身 AI 設計的跨平台 C++ 推理運行時，解決 VLA/WAM 模型在邊緣機器人上部署的延遲與記憶體瓶頸，並提供統一介面支援多種主流模型架構。

## 應用情境與實務影響

機器人開發者可直接將 Pi0、OpenVLA、GR-1 等主流具身模型部署到資源受限的邊緣裝置（Jetson Orin、RK3588、Intel NPU 等），無需依賴 Python 深度學習框架，大幅降低實機部署門檻。

## 補充細節

論文編號 arXiv:2607.02501v3（2026-07-03 提交，2026-07-20 更新 v3）。實驗在 LIBERO 與 RoboTwin 基準上驗證，端到端延遲較 PyTorch 基線降低 2.1-3.8×，準確率損失 <1%。運行時支援即插即用的模型轉換工具鏈，並內建模擬器評估客戶端。專案網站：https://embodied-cpp.github.io，GitHub：https://github.com/tiiuae/Embodied.cpp-edge。

## 維護紀錄

- 收錄日期：2026-08-15
- 最後更新：2026-08-15

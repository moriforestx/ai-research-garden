---
title: "On-Device LLM"
type: concept
research_topic: "AI 綜合動態 / General AI Updates"
keywords:
  - "on-device inference"
  - "edge AI"
  - "privacy-preserving AI"
  - "Apple Foundation Models"
  - "local LLM"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - concept
---

# On-Device LLM

## 基本資訊

- 研究主題：AI 綜合動態 / General AI Updates
- 關鍵字：on-device inference、edge AI、privacy-preserving AI、Apple Foundation Models、local LLM

## 概念概要

On-Device LLM 指直接在使用者端裝置（手機、筆電、平板等）上執行推理的大型語言模型，不需將資料傳送至雲端伺服器。典型參數量在 1B-7B 之間，透過量化、知識蒸餾、架構優化等技術適應裝置端算力與記憶體限制。

## 定義與核心概念

- **裝置端推理**：模型權重與 KV cache 皆駐留於本地記憶體，推理過程不經網路
- **隱私優先**：用戶資料（對話內容、個人文件、位置等）不離開裝置
- **離線可用**：無網路環境下仍可運作
- **低延遲**：消除網路往返時間，首 Token 延遲通常 < 100ms
- **零邊際成本**：開發者無需支付 API 呼叫費用

## 技術原理

1. **模型壓縮**：INT4/INT8 量化、GPTQ/AWQ、動態量化
2. **架構優化**：分組查詢注意力 (GQA)、共享 KV cache、滑動窗口注意力
3. **硬體加速**：神經網路引擎 (ANE/NPU/GPU) 專用算子、金鑰值快取優化
4. **知識蒸餾**：從大模型蒸餾至小模型保留核心能力

## 常見方法與實作方式

- Apple Foundation Models (iOS 26+ / macOS 26+)
- MLX / llama.cpp / MLC LLM (開源推理引擎)
- Google MediaPipe LLM Inference (Android)
- Qualcomm AI Hub Models (Snapdragon)
- Microsoft Phi-3-mini (3.8B, on-device 優化)

## 適用情境

- 個人助理（行程、郵件、筆記）
- 敏感領域 App（醫療記錄、金融帳務、法律文件）
- 離線優先應用（飛行模式、弱網環境）
- 即時工具呼叫（本地資料庫查詢、檔案操作、系統控制）

## 優點與限制

### 優點
- 隱私保護最強
- 離線可用
- 低延遲、無 API 成本
- 個人化微調可在本地進行

### 限制
- 模型容量上限受限於裝置記憶體 (通常 ≤ 8GB 可用)
- 複雜推理、長文脈、多語言能力遜於雲端大模型
- 硬體碎片化：需適配多種晶片 (Apple Silicon, Snapdragon, MediaTek, Intel NPU 等)
- 模型更新需透過 OS 更新或 App 更新分發

## 與相關概念的差異

| 概念 | 差異 |
|------|------|
| Edge AI | 含義更廣，包含 CV、語音等非 LLM 任務 |
| Private Cloud Compute | Apple 混合架構：裝置端優先，複雜任務加密送至私有雲端 |
| Federated Learning | 訓練階段分散式，推理仍可能在雲端 |
| Small Language Models (SLM) | 參數量定義 (≤7B)，不一定部署在裝置端 |

## 相關研究成果

- Apple Intelligence Foundation Language Models (arXiv:2507.13575)
- Phi-3 Technical Report (Microsoft)
- Gemma 2B/7B (Google)
- MobileLLM (Meta)

## 相關工具與專案

- Apple Foundation Models Framework
- MLX (Apple Silicon 優化)
- llama.cpp (跨平台 CPU/GPU 推理)
- MLC LLM (TVM 編譯優化)
- MLX Swift (Swift 介面)

## 相關人物

- Apple Machine Learning Research 團隊
- Microsoft Phi 團隊
- Google Gemma 團隊

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

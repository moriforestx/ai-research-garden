---
title: "vLLM v0.29.0 發布：Model Runner V2 成為預設執行路徑，移除 10 棄用架構、新增 Hy4-preview 與 Qwen3.8-Flash-Next 支援"
type: tool
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-09"
organization: "vLLM Project (PyTorch Foundation)"
source_url: "https://ai-tldr.dev/releases/vllm-v0-29-0"
date_collected: "2026-11-13"
date_updated: "2026-11-13"
tags:
  - ai
  - tool
---

# vLLM v0.29.0 發布：Model Runner V2 成為預設執行路徑，移除 10 棄用架構、新增 Hy4-preview 與 Qwen3.8-Flash-Next 支援

## 基本資訊

- 發布日期：2026-09-09
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://ai-tldr.dev/releases/vllm-v0-29-0

## 概要

vLLM 專案於 2026 年 9 月 9 日發布 v0.29.0，將 Model Runner V2 (MRV2) 設為所有模型的預設執行路徑，結束長期的自願啟用階段。此版本包含 594 次提交、277 位貢獻者（其中 91 位首貢）、移除 Arctic、Chameleon、MPT 等 10 個棄用模型架構，棄用舊式 `python -m vllm.entrypoints.openai.api_server` 入口點改為 `vllm serve`，並新增對騰訊 Hy4-preview（770B/49B MoE）與 Qwen3.8-Flash-Next 的服務支援。MRV2 以更清晰的狀態擁有權、GPU 原生輸入準備、非同步優先設計重構核心執行路徑，帶來更乾淨的代碼與更佳效能。

## 核心價值

完成了歷時數版本的 MRV2 推廣里程碑，確立了統一、模組化、GPU 原生的推理核心為預設值，並同步清理技術債務（移除 10 架構、統一入口點），為生產級推理服務奠定更穩固基礎。

## 應用情境與實務影響

生產部署無需再設定環境變數即可獲得 MRV2 效能優勢；遷移至 `vllm serve` 統一操作介面；新模型支援擴大即時可服務模型庫；架構移除減少維護負擔與潛在相容性問題。Kimi-K3、DeepSeek-V4、Mamba、NemotronH 等前沿模型獲得針對性優化（前綴快取、投機解碼統計、RL 權重同步等）。

## 補充細節

官方 GitHub Release v0.29.0 確認 MRV2 為所有密集模型預設（部分 ROCm 模型暫保留 MRV1）。亮點包括：CUDA 圖記憶體分析自動調整 KV 快取、批次分片採樣降低 logits 記憶體 1/TP、提示嵌入、隱藏狀態提取、投機解碼完整 CUDA 圖調度、DP 同步跳過、Mamba 前綴快取保留內部預填檢查點（TTFT 提升 9-25%）、投機解碼每請求接受率統計、分片 RDT P2P 後端。授權 Apache-2.0。

## 維護紀錄

- 收錄日期：2026-11-13
- 最後更新：2026-11-13

---
title: "GPA v1.5：統一 ASR、TTS 與語音轉換的自回歸音頻基礎模型"
type: tool
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-04-29"
organization: "AutoArk"
source_url: "https://github.com/AutoArk/GPA"
date_collected: "2026-09-22"
date_updated: "2026-09-22"
tags:
  - ai
  - tool
---

# GPA v1.5：統一 ASR、TTS 與語音轉換的自回歸音頻基礎模型

## 基本資訊

- 發布日期：2026-04-29
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://github.com/AutoArk/GPA

## 概要

AutoArk 於 2026 年 4 月 29 日發布 GPA v1.5，單一自回歸 Transformer 統一語音識別 (ASR)、語音合成 (TTS) 與語音轉換 (VC) 三大任務，達 near-SOTA 效能。模型採純離散語音標記與共享骨幹，透過提示詞隱式指定任務，無需切換模型。同步釋出 ONNX Runtime 部署包，支援 CLI、FastAPI 服務與瀏覽器 UI。arXiv:2601.10770 (2026-01) 技術報告詳述架構與聯合多任務訓練細節。

## 核心價值

首個在單一輕量自回歸架構下同時達 near-SOTA ASR/TTS 效能的開源統一音頻模型，ONNX 原生部署大幅降低邊緣與生產環境門檻。

## 應用情境與實務影響

開發者可用單一模型替換傳統 ASR+TTS+VC 管線，減少模型管理複雜度與延遲；ONNX 支援使瀏覽器、移動端、嵌入式設備均可直接部署。

## 補充細節

架構：共享 Transformer 骨幹 + 離散音頻標記碼本。訓練數據：Emilia 數據集混合自建語料。基準：TTS 串流 RTF、ASR 串流 TTFT/P99 延遲數據公開。Hugging Face: Audio8/GPA。GitHub: AutoArk/GPA (Apache-2.0)。VC 功能規劃中。

## 維護紀錄

- 收錄日期：2026-09-22
- 最後更新：2026-09-22

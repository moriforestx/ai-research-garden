---
title: "VoxCPM2：開源多語言可控語音生成基礎模型，支援 30 語言、自然語言聲音設計、高保真克隆"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-05"
organization: "OpenBMB"
source_url: "https://arxiv.org/abs/2606.06928"
date_collected: "2026-08-01"
date_updated: "2026-08-01"
tags:
  - ai
  - paper
---

# VoxCPM2：開源多語言可控語音生成基礎模型，支援 30 語言、自然語言聲音設計、高保真克隆

## 基本資訊

- 發布日期：2026-06-05
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2606.06928

## 概要

OpenBMB（清華 NLP 與 ModelBest）發布 VoxCPM2 技術報告，提出完全開源的多語言可控語音生成基礎模型。擴展 VoxCPM 的階層式擴散自迴歸範式，在單一 2B 參數骨幹上統一 30 語言、9 中文方言、自然語言聲音設計、風格可控聲音克隆、高保真續作克隆。基於 MiniCPM-4，訓練資料超過 200 萬小時多語言語音，輸出 48kHz 錄音室級音質，Apache 2.0 許可證。RTX 4090 上 RTF 約 0.30，Nano-vLLM 加速後約 0.13。代碼、權重、Demo 全開源。

## 核心價值

首個在單一開源模型整合多語言、聲音設計、可控克隆、續作克隆的 TTS 基礎模型，證明 tokenizer-free 擴散自迴歸範式可達商業級音質與控制力，大幅降低高品質 TTS 部署門檻。

## 應用情境與實務影響

開發者可自行部署商業級多語言 TTS，無需依賴 ElevenLabs 等閉源 API；語音設計功能支援自然語言描述生成聲音，無需參考音頻；Apache 2.0 許可證允許商業使用與二次開發。

## 補充細節

arXiv:2606.06928v1，提交於 2026-06-05。類別：cs.SD、eess.AS。作者：Zhou Yixuan 等（OpenBMB）。架構：LocEnc → TSLM → RALM → LocDiT 四階段管線，完全在 AudioVAE V2 潛空間操作。骨幹 MiniCPM-4（2B 參數），LM token rate 6.25 Hz，max seq len 8192。基準測試：Minimax-MLS 英文聲音相似度 85.4%（ElevenLabs 61.3%）。GitHub: OpenBMB/VoxCPM，HuggingFace: openbmb/VoxCPM2。

## 維護紀錄

- 收錄日期：2026-08-01
- 最後更新：2026-08-01

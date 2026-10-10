---
title: "VOICE-AE：從環境臨床音訊自動評分 CTCAE，結合語音辨識與大型語言模型"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-10-10"
organization: "多機構醫學中心合作"
source_url: "https://www.nature.com/articles/s41746-026-03373-z"
date_collected: "2026-10-11"
date_updated: "2026-10-11"
tags:
  - ai
  - paper
---

# VOICE-AE：從環境臨床音訊自動評分 CTCAE，結合語音辨識與大型語言模型

## 基本資訊

- 發布日期：2026-10-10
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://www.nature.com/articles/s41746-026-03373-z

## 概要

研究團隊開發 VOICE-AE 系統，自動從醫療環境的環境音訊中擷取不良事件，並對應 CTCAE（癌症治療不良事件通用術語標準）進行分級。管線整合語音辨識（Whisper-large-v3）、說話人分離與 LLM（GPT-4o）進行臨床實體抽取與分級推理。於 127 段真實臨床錄音驗證，宏平均 F1 達 0.82，顯著優於人工基準。已於 2026-10-10 發表於 npj Digital Medicine。

## 核心價值

展示端到端語音+LLM 管線在高風險醫療場景的實用可行性，為自動化藥物警訊與臨床試驗監測奠定技術基石。

## 應用情境與實務影響

醫院、CRO 與製藥廠可部署此類系統降低人工稽核成本、提升不良事件回報完整度與即時性；架構可遷移至其他臨床編碼任務（如 ICD-10、MedDRA）。

## 補充細節

DOI: 10.1038/s41746-026-03373-z。Received: 2026-04-10，Accepted: 2026-09-26，Published online: 2026-10-10。作者來自多間歐美醫學中心與 AI 實驗室。代碼與去識別化數據集已公開於 GitHub。

## 維護紀錄

- 收錄日期：2026-10-11
- 最後更新：2026-10-11

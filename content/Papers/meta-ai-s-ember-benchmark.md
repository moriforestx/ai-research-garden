---
title: "S-EMBER: A Large-Scale Benchmark for Streaming Egocentric Memory Retrieval"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-07-13"
organization: "Meta AI"
source_url: "https://ai.meta.com/research/publications/s-ember-a-large-scale-benchmark-for-streaming-egocentric-memory-retrieval"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - paper
---

# S-EMBER: A Large-Scale Benchmark for Streaming Egocentric Memory Retrieval

## 基本資訊

- 發布日期：2026-07-13
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://ai.meta.com/research/publications/s-ember-a-large-scale-benchmark-for-streaming-egocentric-memory-retrieval

## 概要

Meta AI 於 2026 年 7 月 13 日發表 S-EMBER (Streaming Egocentric Memory Benchmark for Episodic Retrieval) 基準測試，針對可穿戴裝置第一人稱視角的長時程記憶檢索任務。資料集包含 3,141 支影片、總計 388 小時的有機活動內容，皆透過 Ray-Ban Meta 智慧眼鏡實際拍攝。基準定義「接地式串流情境記憶檢索」，要求模型在連續串流中由視覺事件觸發主動回溯，並對 9,448 組問答對進行精確時序定位與視覺證據驗證。實驗發現「定位悖論」：語意推理能力隨參數規模提升，但時序定位精度卻成為不隨模型大小、解析度或幀率改善的架構瓶頸。

## 核心價值

S-EMBER 首次以硬體真實資料建立串流式情境記憶基準，揭示前沿模型在長時程第一人稱視訊中的時序定位能力為關鍵瓶頸，為下一代可穿戴 AI 代理人奠定評測基石。

## 應用情境與實務影響

可穿戴 AI 助理、AR 眼鏡、機器人長期記憶系統的研發團隊可直接使用 S-EMBER 進行模型選型與架構改進；9,448 組 QA 對與 388 小時真實佩戴資料提供標準化評測管線，加速產業界從離線檢索轉向串流式主動回溯範式。

## 補充細節

資料集採 CC-BY-4.0 授權釋出，包含影片、標註、評測腳本與基線模型權重。作者團隊來自 Meta AI Research（FAIR）與 Reality Labs，第一作者 Xiaodong Wang、Xuanyi Zhao，通訊作者 Wen-tau Yih。論文已上傳 arXiv（arXiv:2607.xxxxx），並同步發布 GitHub 復現代碼。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

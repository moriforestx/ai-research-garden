---
title: "Microsoft releases BitNet Text Embeddings: 1-bit embedding models with competitive performance and 2.28x CPU throughput improvement"
type: technical-development
research_topic: "大型語言模型與自然語言處理 / LLM & NLP"
published_date: "2026-07-15"
organization: "Microsoft"
source_url: "https://huggingface.co/microsoft/bitnet-embedding-0.6b"
date_collected: "2026-09-04"
date_updated: "2026-09-04"
tags:
  - ai
  - technical-development
---

# Microsoft releases BitNet Text Embeddings: 1-bit embedding models with competitive performance and 2.28x CPU throughput improvement

## 基本資訊

- 發布日期：2026-07-15
- 研究主題：大型語言模型與自然語言處理 / LLM & NLP
- 主要來源：https://huggingface.co/microsoft/bitnet-embedding-0.6b

## 概要

微軟 BitNet 團隊於 2026 年 7 月 15 日發布首個 1-bit 文字嵌入模型系列 BitNet-Embeddings，包含 0.6B 和 270M 參數版本。該模型使用三元權重和量化激活函數，在保持與全精度教師模型相近的嵌入品質（MMTEB 基準測試中僅低 0.35 點）的同時，實現 2.28x 的 CPU 推理吞吐量提升，顯著降低記憶體與計算成本。

## 核心價值

極低位元（1-bit）文字嵌入模型，在效能與效率間達成突破性平衡。

## 應用情境與實務影響

使得文字嵌入工作負載可在資源受限環境（如邊緣設備、行動裝置）上以極低成本運行，適合大規模檢索、分群、語義相似度計算及多語言應用場景。

## 補充細節

BitNet-Embedding-0.6B 使用解碼器 seule 架構配合最後標記匯集和 L2 正規化生成稠密文字嵌入。模型經過持續對比預訓練與監督對比微調，結合相似度分布蒸餾和注意力關係蒸餾來對齊全精度教師模型。在 MMTEB (eng, v2) 基準測試中達到 67.60 平均得分（FP16 教師模型為 67.95），在 CPU 上（8 線程）達到 870.90 個標記/秒的推理速度，比FP16 基線快 2.28 倍。模型支援多種存儲精度（1-bit, 2-bit, 4-bit, 8-bit），可根據應用場景靈活權衡效能與儲存成本。

## 維護紀錄

- 收錄日期：2026-09-04
- 最後更新：2026-09-04

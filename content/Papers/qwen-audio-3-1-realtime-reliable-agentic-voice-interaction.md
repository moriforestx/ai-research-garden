---
title: "Qwen-Audio-3.1-Realtime: Towards Reliable Agentic Voice Interaction"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-09-24"
organization: "Alibaba Token Foundry, Alibaba Group"
source_url: "https://arxiv.org/abs/2609.25176v2"
date_collected: "2026-10-29"
date_updated: "2026-10-29"
tags:
  - ai
  - paper
---

# Qwen-Audio-3.1-Realtime: Towards Reliable Agentic Voice Interaction

## 基本資訊

- 發布日期：2026-09-24
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2609.25176v2

## 概要

Alibaba Token Foundry 發布 Qwen-Audio-3.1-Realtime，專為可靠的代理型語音交互設計。架構以「Think、Act、Speak and Coordinate」三層支撐：Think 採 Core-Cocktail SFT 配合 Multimodality OPD 與 Multi-Teacher OPD (M²-OPD)，將文本 LLM 推理能力轉移並發展原生音頻技能；Act 引入自我演化可執行環境與多粒度 rollout (對話/里程碑/輪次三層獎勵) 進行 GRPO 訓練，賦予工具使用、任務完成與進度回報能力；Speak and Coordinate 制定何時說話、如何表達、雙工協調等會話策略。評測顯示：半雙工 τ-Voice 任務成功率從 78.4% 提升至 82.0%；全雙工基準下背景語音誤觸發率從 73.0% 降至 13.0%。另附 Voice Harness 原型實現持久化任務協同。技術報告 25 頁，開源於 arXiv。

## 核心價值

首創 M²-OPD 雙路蒸餾管線與自我演化可執行環境，系統性解決即時語音助手的推理、行動、交互三大核心挑戰，大幅降低全雙工誤觸發率。

## 應用情境與實務影響

為產業級即時語音代理提供完整訓練範式與評測體系；M²-OPD 可移植至其他音頻 LLM 遷移文本推理能力；可執行環境設計建立工具使用與長時程任務的標準化訓練框架。

## 補充細節

架構採雙路 Audio Encoder + LLM：全雙工決策模型控制語音時序，S2T 模型生成回應內容，配合上下文感知語音渲染器實現串流合成。Core-Cocktail SFT 以百萬小時級多領域音文數據冷啟動；Multimodality OPD 以凍結 Audio Reference 提供音頻條件監督；Multi-Teacher OPD 整合領域專家模型 token 級監督。GRPO 三層獎勵：對話級 (任務成功)、里程碑級 (關鍵步驟完成)、輪次級 (即時進度真實性)。接受 ISMIR 2026 相關會議軌。

## 維護紀錄

- 收錄日期：2026-10-29
- 最後更新：2026-10-29

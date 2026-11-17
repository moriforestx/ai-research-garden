---
title: "Rethinking KV Cache Eviction for Agentic LLM Serving"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-30"
organization: "未明確列出機構"
source_url: "https://arxiv.org/abs/2611.00391"
date_collected: "2026-11-18"
date_updated: "2026-11-18"
tags:
  - ai
  - paper
---

# Rethinking KV Cache Eviction for Agentic LLM Serving

## 基本資訊

- 發布日期：2026-10-30
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2611.00391

## 概要

針對代理型 LLM 服務系統的 KV 快取記憶體壓力問題，提出 Penelope 系統。現有機制通常從序列兩端驅逐 KV 以保留前綴共享，但代理工作負載會跨多輪重複重用長歷史。重新計算序列末端附近 token 的 KV 快取成本顯著高於早期 token（因注意力計算涉及更長歷史）。Penelope 策略：保留共享前綴，從剩餘歷史開頭驅逐 KV 快取同時保留快取後綴。聯合設計驅逐策略、KV 重計算與統一 GPU-CPU 兩層快取管理。在 SGLang 實作，於三種 Qwen3 模型規模用真實代理軌跡評測：僅 GPU 快取下 mean TTFT 降至多 60%、作業完成時間降至多 37%；雙層 GPU-CPU 快取下分別降至多 76% 與 60%。

## 核心價值

首個針對代理工作負載特徵（長歷史重用、末端重計算昂貴）優化的 KV 快取驅逐與多層管理方案，大幅降低代理型 LLM 服務延遲。

## 應用情境與實務影響

直接適用於生產級代理服務平台（SGLang、vLLM 等），減少 GPU 記憶體壓力、降低服務成本、提升多輪對話代理的響應速度。

## 補充細節

提交日期：2026-10-30 (v1)。作者：Jiakun Fan 等。實作於 SGLang，代碼開源。三種 Qwen3 模型規模驗證。

## 維護紀錄

- 收錄日期：2026-11-18
- 最後更新：2026-11-18

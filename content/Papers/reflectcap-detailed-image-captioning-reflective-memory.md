---
title: "ReflectCAP: Detailed Image Captioning with Reflective Memory"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-10"
organization: "Adobe Research"
source_url: "https://research.adobe.com/publication/reflectcap-detailed-image-captioning-with-reflective-memory"
date_collected: "2026-10-19"
date_updated: "2026-10-19"
tags:
  - ai
  - paper
---

# ReflectCAP: Detailed Image Captioning with Reflective Memory

## 基本資訊

- 發布日期：2026-09-10
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://research.adobe.com/publication/reflectcap-detailed-image-captioning-with-reflective-memory

## 概要

Adobe Research 發表 ReflectCAP，針對大型視覺語言模型 (LVLM) 圖像描述中的「幻覺」與「遺漏」雙重難題，提出反思記憶導向描述法。多代理管線自動分析目標 LVLM 的系統性錯誤與盲區，提煉為可復用的結構化反思筆記，推理時雙向引導模型避開錯誤、補齊遺漏。在 GPT-4.1、Qwen、InternVL 等 8 款 LVLM 上實驗，ReflectCAP 同時提升事實性與覆蓋率，達到 Pareto 前沿，於 CapArena-Auto 對戰評測中大幅超越基準。

## 核心價值

首創「反思記憶」機制將模型的歷史錯誤模式轉化為推理期導引，無需微調即可即插即用於任意 LVLM；結構化反思筆記同時編碼「避免清單」與「關注清單」，破解事實性與覆蓋率的長期權衡。

## 應用情境與實務影響

產業界可直接套用於現有 LVLM 服務，零訓練成本提升描述品質；適用於醫療影像報告、自動駕駛場景描述、內容審核等高可信度需求場景；多代理分析管線可遷移至其他生成任務的自我改進。

## 補充細節

ECCV 2026 接收（2026-09-10 發布）。作者 Kyungmin Min、Minbeom Kim、Kang-il Lee、David Seunghyun Yoon、Kyomin Jung (Adobe Research / Seoul National University)。arXiv:2604.12357v1。實驗涵蓋 CapArena-Auto、CHAIR、F1@K、Coverage@K 等基準；反思筆記生成成本約 200 次 API 呼叫，推理零額外開銷。

## 維護紀錄

- 收錄日期：2026-10-19
- 最後更新：2026-10-19

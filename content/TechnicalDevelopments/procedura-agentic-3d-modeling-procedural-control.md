---
title: "Procedura: Agentic 3D Modeling with Procedural Control"
type: technical-development
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-08-26"
organization: "未明確標示單一機構，作者來自多個研究團隊"
source_url: "https://arxiv.org/abs/2608.26238"
date_collected: "2026-08-30"
date_updated: "2026-08-30"
tags:
  - ai
  - technical-development
---

# Procedura: Agentic 3D Modeling with Procedural Control

## 基本資訊

- 發布日期：2026-08-26
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2608.26238

## 概要

提出 Procedura，一個以程式碼表示 3D 形狀的代理框架。利用 LLM 的編碼能力，將物件規劃為程序化組裝圖，逐部件撰寫參數化程式，並透過編譯、配合與連通性檢查驗證每個部件。再引入解耦的視覺評論者逐步修正組裝。輸出為可編輯、具部件結構的程式，並攜帶材質與經模擬驗證的關節關係。

## 核心價值

首個實現「3D 形狀即程式碼」的代理系統，輸出可編輯的程序化組裝程式，解決原生 3D 生成器輸出網格軟、無部件分解、不可編輯的核心痛點。

## 應用情境與實務影響

適用於 CAD、機械設計、遊戲資產製作、機器人抓取規劃等需精確幾何與可編輯性的場景；在 P3D-Bench 與 MechBench-36 基準上超越所有既有 3D 代碼代理與原生生成器。

## 補充細節

專案頁面：https://spatiaos.github.io/projects/procedura/；提交日期 2026-08-26 (arXiv:2608.26238v1)；屬 cs.CV、cs.GR 跨領域。

## 維護紀錄

- 收錄日期：2026-08-30
- 最後更新：2026-08-30

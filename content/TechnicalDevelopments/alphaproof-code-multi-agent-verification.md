---
title: "Google DeepMind 發布 AlphaProof Code：多代理 AI 形式化軟體驗證框架"
type: technical-development
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-11-10"
organization: "Google DeepMind"
source_url: "https://deepmind.google/blog/introducing-alphaproof-code"
date_collected: "2026-11-23"
date_updated: "2026-11-23"
tags:
  - ai
  - technical-development
---

# Google DeepMind 發布 AlphaProof Code：多代理 AI 形式化軟體驗證框架

## 基本資訊

- 發布日期：2026-11-10
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://deepmind.google/blog/introducing-alphaproof-code

## 概要

Google DeepMind 於 2026-11-10 發布 AlphaProof Code，一個多代理 AI 框架，用於形式化軟體規格撰寫與驗證。框架包含三大組件：(1) 人類引導代理協助撰寫 Lean 規格、(2) AArch64 機器碼的形式化語意、(3) 自主證明代理團隊，其證明僅在 Lean 核心檢查通過核准規格後才被接受。首次實戰應用於驗證 libsignal（Signal 協定參考實作）的關鍵安全屬性，在機器碼層級生成約 650 萬行機器檢查證明，建立在約 2.6 萬行受信任基礎上。工作由 5 人團隊在 4 週內完成，規格過程中捕獲兩個重新引入的歷史錯誤。證明流程分三階段：規格草擬與核准、編譯機器碼於 Lean 處理器模型運行、證明團隊生成經閘門驗證的證明。

## 核心價值

首個在真實密碼學程式碼庫上實現端到端代理輔助形式化驗證的系統，將傳統需大量人力的機器碼級驗證自動化

## 應用情境與實務影響

高風險程式碼路徑（密碼學、支付流程、安全關鍵邏輯）的自動化形式化驗證；CI/CD 整合的安全合規審查；Signal 協定核心屬性的機器檢查證明，保護數十億用戶私密通訊

## 補充細節

專案頁面：https://google-deepmind.github.io/code-verification。使用 Gemini 4 Carbon 作為基礎模型。Lean 為數學證明編程語言，其核心檢查器為信任基礎。AArch64 為 64 位元 ARM 指令集，涵蓋幾乎所有 Android 手機。代理團隊包含規格撰寫代理與多個自主證明代理。

## 維護紀錄

- 收錄日期：2026-11-23
- 最後更新：2026-11-23

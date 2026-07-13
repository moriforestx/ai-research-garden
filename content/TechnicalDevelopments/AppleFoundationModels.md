---
title: "Apple Foundation Models Framework: On-Device LLM with Tool Calling"
type: technical-development
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-06-09"
organization: "Apple"
keywords:
  - "Foundation Models framework"
  - "on-device LLM"
  - "tool calling"
  - "Apple Intelligence"
  - "WWDC 2026"
  - "Private Cloud Compute"
source_url: "https://developer.apple.com/documentation/foundationmodels"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - technical-development
---

# Apple Foundation Models Framework: On-Device LLM with Tool Calling

## 基本資訊

- 發布組織：Apple
- 發布日期：2026-06-09 (WWDC 2026)
- 研究主題：AI 綜合動態 / General AI Updates
- 關鍵字：Foundation Models framework、on-device LLM、tool calling、Apple Intelligence、WWDC 2026、Private Cloud Compute
- 主要來源：https://developer.apple.com/documentation/foundationmodels

## 動態概要

Apple 在 WWDC 2026 發布 Foundation Models 框架，提供原生 Swift API 直接存取裝置端 30 億參數語言模型。模型專為 Apple Intelligence 優化，支援結構化輸出（@Generable macro）、工具呼叫（Tool protocol）、圖文理解等能力。推理完全在裝置端執行，網路不在呼叫路徑中。

## 技術背景

延續 2025 年推出的 Apple Intelligence 基礎模型（~3B 參數裝置端模型 + PT-MoE 伺服器模型），2026 年將裝置端模型封裝為 Foundation Models 框架，開放第三方 App 直接調用。

## 主要更新內容

1. **Foundation Models 框架**：Swift 原生 API，`SystemLanguageModel.default` 提供預設模型實例
2. **LanguageModelSession**：管理對話狀態、上下文與工具呼叫的會話物件
3. **@Generable macro**：編譯期保證模型輸出符合自訂資料結構
4. **Tool protocol**：自訂工具讓模型呼叫本地資料庫、網路服務或 App 功能
5. **隱私優先**：完全裝置端推理，無網路傳輸

## 涉及技術

- 裝置端 LLM 推理優化 (Apple Silicon)
- 結構化輸出約束生成
- 工具呼叫協定
- Private Cloud Compute 混合推理架構

## 與既有技術的差異

| 特性 | Foundation Models | 傳統雲端 LLM API |
|------|------------------|------------------|
| 推理位置 | 裝置端 | 雲端 |
| 網路需求 | 無 | 必要 |
| 隱私性 | 高 (資料不出裝置) | 視供應商政策 |
| 延遲 | 低 (本地推理) | 視網路情況 |
| 成本 | 免費 (用戶裝置算力) | 按 Token 計費 |

## 潛在應用與影響

- 離線優先的 AI App 體驗
- 敏感資料處理（醫療、金融、個人筆記）
- 即時工具呼叫（行程安排、郵件撰寫、程式碼生成）
- 降低開發者整合 LLM 的門檻與成本

## 限制與待確認事項

- 僅支援 Apple Intelligence 相容裝置 (iPhone 15 Pro 以降、M 系列晶片 Mac/iPad)
- 模型能力固定為 ~3B 參數，複雜推理任務可能不足
- 僅限 Apple 平台，跨平台需另行方案
- 中文等非英語語言表現官方未公開詳細基準

## 相關工具與專案

- Foundation Models 文件：https://developer.apple.com/documentation/foundationmodels
- WWDC 2026 Apple Intelligence 指南：https://developer.apple.com/wwdc26/guides/apple-intelligence

## 相關研究成果

- Apple Intelligence Foundation Language Models Tech Report 2025 (arXiv:2507.13575)

## 相關概念

- 裝置端 AI
- 私有雲端運算
- 工具增強語言模型
- 結構化輸出

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

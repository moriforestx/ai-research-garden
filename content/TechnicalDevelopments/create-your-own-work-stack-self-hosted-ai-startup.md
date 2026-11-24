---
title: "Create Your Own Work Stack: Deploying Self-hosted AI and Tooling in a Tech Startup"
type: technical-development
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-11-05"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.08116"
date_collected: "2026-11-25"
date_updated: "2026-11-25"
tags:
  - ai
  - technical-development
---

# Create Your Own Work Stack: Deploying Self-hosted AI and Tooling in a Tech Startup

## 基本資訊

- 發布日期：2026-11-05
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2611.08116

## 概要

此經驗報告記錄 Grayhat Developers（一家 AI 密集型軟體新創）部署混合式自架 AI 技術棧的完整過程。初衷為降低商用 AI 成本（Claude/Codex 月費約 325 美元、259 億 tokens），嘗試以本地開源模型替代商用編碼代理，發現效能與推理速度不足，轉而採用混合架構：商用代理負責複雜任務，本地模型處理低複雜度任務、組織資訊檢索、與自架工具同步。自架工具鏈含 Outline（知識庫）、Plane（專案管理）、ERPNext（ERP）、Authentik（認證）、Coolify（部署）、MCP 伺服器（AI-工具連接）。關鍵發現：分散式本地部署因 UX 摩擦導致採用率極低，改為集中式配置部署後顯著改善。結論：本地推論最適合作為混合架構一環，依能力需求、成本、上下文要求、操作敏感度分配任務，而非全盤取代商用 AI。

## 核心價值

提供真實產業級部署案例，量化成本權衡、架構決策演進、採用障礙與解決方案，打破「自架即省錢」迷思，確立混合式任務分配為 2026 年自架 AI 的務實最佳實踐。

## 應用情境與實務影響

為中小型團隊評估自架 AI 可行性提供決策參考：硬體規格、工具選型、部署拓撲、成本模型、遷移路徑。強調 UX 設計對採用率的決定性影響，提醒避免過度工程化。MCP 伺服器模式可推廣至企業內部 AI-工具整合標準。

## 補充細節

公司：Grayhat Developers。硬體：推理機（2×RTX 4090、128GB RAM）、應用機（Coolify 部署 Outline/Plane/ERPNext/Authentik）。模型：本地嘗試 Llama-3.1-70B、Qwen2.5-Coder-32B，最終採用混合。成本對比：商用月 325 美元 vs 自架硬體折舊+電力估約 180 美元/月（含機會成本）。採用率指標：分散式部署 <15% 團隊活躍使用，集中式配置後 >70%。失敗教訓：本地模型上下文窗口限制、工具調用可靠性、團隊習慣遷移阻力。開源：配置腳本、MCP 伺服器實作、硬體清單。

## 維護紀錄

- 收錄日期：2026-11-25
- 最後更新：2026-11-25

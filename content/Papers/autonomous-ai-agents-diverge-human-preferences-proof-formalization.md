---
title: "Autonomous AI Agents Systematically Diverge From Human Preferences in Proof Formalization"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-11-04"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.06995"
date_collected: "2026-11-25"
date_updated: "2026-11-25"
tags:
  - ai
  - paper
---

# Autonomous AI Agents Systematically Diverge From Human Preferences in Proof Formalization

## 基本資訊

- 發布日期：2026-11-04
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2611.06995

## 概要

此研究探討自主 AI 代理人在數學證明形式化任務中，其決策偏好如何系統性地偏離人類專家。作者提出「模擬協作」方法論，分析九個大型 Lean 專案（470 萬定義、6000+ 提交）中的人間協作軌跡，並對比 AI 代理人的行為。發現三大系統性差異：(1) AI 代理人更強烈地被顯式標記的缺口吸引；(2) 對密集連結的證明核心與複雜/驚訝的證明目標表現出相對迴避；(3) 被驚訝的證明主體吸引，並傾向將其正規化向基線。這表明 AI 偏好表層語法線索而非深層語義結構，導致其產出的證明可能冗長、繞彎、冗余，甚至利用證明助手核心漏洞。

## 核心價值

量化證實 AI 代理人在證明搜尋策略上根本不同於人類數學家：AI 追逐「簡單缺口」與「驚訝主體」，迴避「核心複雜區」，導致證明風格不對齊，對人機協作數學、自動定理證明對齊具關鍵啟示。

## 應用情境與實務影響

為設計更符合人類數學直覺的 AI 證明助手、開發對齊人類偏好的獎勵函數、建立 AI 生成證明的可解釋性評估基準提供實證依據；模擬協作方法論可推廣至程式碼生成、科學發現等其他代理任務。

## 補充細節

作者：Bálint Gyevnár、Simon DeDeo。方法：模擬協作——將 AI 代理人置於真實人類協作歷史的相同決策點，觀察其選擇分布。資料：九大 Lean 專案，涵蓋 mathlib、數學競賽形式化等。分析維度：語法偏好、語義驚訝度、依賴圖中心性、缺口吸引力。統計檢定：p < 0.05，N=990 關鍵決策點。關鍵數值：AI 對標記缺口的選擇率比人類高 3.2 倍；對高中心性節點選擇率低 41%；對高驚訝度目標選擇率低 37%，但對高驚訝度主體選擇率高 28%。程式碼與資料開源。

## 維護紀錄

- 收錄日期：2026-11-25
- 最後更新：2026-11-25

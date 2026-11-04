---
title: "Do Coding Agents Catch Their Own Bugs? (They Don't.)"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-10-31"
organization: "arXiv"
source_url: "https://arxiv.org/abs/2611.01181"
date_collected: "2026-11-05"
date_updated: "2026-11-05"
tags:
  - ai
  - paper
---

# Do Coding Agents Catch Their Own Bugs? (They Don't.)

## 基本資訊

- 發布日期：2026-10-31
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2611.01181

## 概要

提出 Foresight-SWE 基準測試，衡量程式設計智能體是否能預見並解決軟體工程任務中未明確規定的潛在問題（如前瞻性考慮漏洞或 Bug）。包含 212 樣本，橫跨 4 種語言、35 個熱門開源倉庫，每樣本含兩個 PR（第二個修正第一個引入的缺陷）。定義「預見解決率」(FRR) 為同時完成原任務並避免後續 PR 識別缺陷的比例。

## 核心價值

評估 11 個大型語言模型，FRR 僅 6.13% 到 24.53%，顯示模型多數無法解決首個 PR 變更引入的問題。揭示編碼場景下模型訓練與對齊的缺口，以及程式碼審查工具需改進以實現更安全編碼。

## 應用情境與實務影響

將評估導向前瞻性缺陷預防，對 AI 輔助程式碼生成的生產部署可靠性至關重要。提供基準推動更安全的編碼智能體開發。

## 補充細節

作者：Shaswat Patel 等 5 人。arXiv:2611.01181v1，2026-10-31 提交。主題：Software Engineering (cs.SE)。授權：CC BY 4.0。

## 維護紀錄

- 收錄日期：2026-11-05
- 最後更新：2026-11-05

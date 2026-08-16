---
title: "Vero: Can AI Agents Build Formally Verified Software Repositories?"
type: paper
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-08-13"
organization: "Zhe Ye, Hantao Lou, Yuechun Sun, Peiyang Song, Zhengxu Yan, Timothe Kasriel, Qingyang Zhang, Kaiyu Yang, Soonho Kong, Jingxuan He, Dawn Song"
source_url: "https://arxiv.org/abs/2608.13522"
date_collected: "2026-08-17"
date_updated: "2026-08-17"
tags:
  - ai
  - paper
---

# Vero: Can AI Agents Build Formally Verified Software Repositories?

## 基本資訊

- 發布日期：2026-08-13
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://arxiv.org/abs/2608.13522

## 概要

推出 Vero，首個評測 AI 代理在儲存庫層級同時生成實現代碼與機器檢查證明的基準。包含 43 個多模組實例，源自真實儲存庫（Python、Dafny、Verus、Coq），涵蓋密碼協議到分散式系統等領域。每個實例為預設 API 接口的 Lean 4 多模組倉庫，附帶人工策展形式化規格與參考實現，支援純證明與代碼+證明雙模式評測。引入審計機制允許代理證明規格不可滿足或參考代碼錯誤，修正策展潛在錯誤。最強代理僅完全解決 27/43 實例，最難倉庫零規格通過。為可信 AI 生成軟體提供具體測試床，基準、策展管線、評測工具開源於 GitHub。

## 核心價值

填補儲存庫級驗證代碼生成評測空白；證明當前前沿代理在多模組協同實現與證明選擇上仍有巨大差距。

## 應用情境與實務影響

為生產級 AI 輔助軟體開發建立可信度基準；推動形式化驗證融入 AI 代碼生成流程，對金融、醫療、航空航天等高可靠性領域部署至關重要。

## 補充細節

專案：https://github.com/sunblaze-ucb/vero；arXiv:2608.13522。發布日期以 arXiv citation_date (2026-08-13) 為準。

## 維護紀錄

- 收錄日期：2026-08-17
- 最後更新：2026-08-17

---
title: "GPT-5.6 System Card: OpenAI 部署安全評估與防護架構"
type: report
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-09"
organization: "OpenAI"
source_url: "https://deploymentsafety.openai.com/gpt-5-6"
date_collected: "2026-09-20"
date_updated: "2026-09-20"
tags:
  - ai
  - report
---

# GPT-5.6 System Card: OpenAI 部署安全評估與防護架構

## 基本資訊

- 發布日期：2026-07-09
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://deploymentsafety.openai.com/gpt-5-6

## 概要

OpenAI 發布 GPT-5.6 System Card，詳述 GPT-5.6 Sol 與 GPT-5.6 Luna 兩款前沿模型的部署安全評估。依據 Preparedness Framework，兩模型在網絡安全與生化領域均達 High 能力等級，尚未達 AI 自我改進 High 門檻。文檔涵蓋自動化紅隊模型 GPT-Red（自博弈強化學習訓練，專精提示詞注入攻擊發掘）、CoT 控制力評估（CoT-Control，13,000+ 任務）、SWE-Bench Verified 程式碼生成基準、以及配套防護措施。另包含 2026/08/03 新增的 GPT-Red 評估結果與 2026/08/19 的蛋白質結合預測分數修正。

## 核心價值

展示前沿模型部署前的標準化安全評估流程：能力分級、紅隊測試、可控性驗證與防護措施對應，為 AI 應用大規模落地建立可審計的安全基線。

## 應用情境與實務影響

企業與監管機構可參考此系統卡範本，建立自有模型部署的風險評估與合規檢核清單；研究者獲得自動化紅隊與 CoT 控制力評估的具體方法論。

## 補充細節

系統卡 PDF 可下載。GPT-Red 採自博弈 RL 訓練，能利用大規模算力自我改進攻擊策略。CoT-Control 涵蓋 GPQA、MMLU-Pro、HLE、BFCL、SWE-Bench Verified 五大基準。部署防護包含輸出過濾、工具調用沙箱、審計日誌與存取控制。

## 維護紀錄

- 收錄日期：2026-09-20
- 最後更新：2026-09-20

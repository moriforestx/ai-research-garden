---
title: "Loop-Back Authority in LLM Agent Teams: A Paired Experiment on Flat and Hierarchical Coordination"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-09-13"
organization: "獨立研究者"
source_url: "https://arxiv.org/abs/2609.14767"
date_collected: "2026-10-02"
date_updated: "2026-10-02"
tags:
  - ai
  - paper
---

# Loop-Back Authority in LLM Agent Teams: A Paired Experiment on Flat and Hierarchical Coordination

## 基本資訊

- 發布日期：2026-09-13
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2609.14767

## 概要

本文以配對實驗檢驗 LLM 代理團隊中「循環權威」的效果。實驗固定五個代理的角色、提示、工具、模型與資料，僅操縱一個變因：Manager 是否可退回 Worker 輸出並要求修訂。跨 43 組配對產出與 86 次商業智慧報告任務，五模型評審團與規格檢查一致顯示：扁平組織在 Utility (d=0.42, p=0.009) 與 Writing Clarity (d=0.34, p=0.030) 顯著優於階層組織；階層版本多花 51.5% token 卻無品質增益，且導致修訂迴路中 hedging 增加 53%、每輪修訂使 Writing Clarity 下降 0.14 分。

## 核心價值

實證推翻經典組織理論預測：在開放式語言生成任務中，階層式循環權威反而損害產出品質與成本效率，扁平協作更優。

## 應用情境與實務影響

對設計多代理 LLM 系統（如 AutoGPT、LangGraph、CrewAI 等）的協作架構具直接指導意義；建議在開放式任務中預設扁平協作，謹慎引入監督層。

## 補充細節

arXiv:2609.14767v1 [cs.MA]，提交日期 2026-09-13。作者：Burak Agachan、Max van Duijn、Amirhossein Zohrehvand。屬多代理系統與組織行為交叉研究。

## 維護紀錄

- 收錄日期：2026-10-02
- 最後更新：2026-10-02

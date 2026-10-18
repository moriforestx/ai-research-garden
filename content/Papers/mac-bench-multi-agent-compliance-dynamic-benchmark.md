---
title: "Beyond Goodhart's Law: A Dynamic Benchmark for Evaluating Compliance in Multi-Agent Systems"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-06-10"
organization: "arXiv (multi-institution)"
source_url: "https://arxiv.org/abs/2606.07805"
date_collected: "2026-10-19"
date_updated: "2026-10-19"
tags:
  - ai
  - paper
---

# Beyond Goodhart's Law: A Dynamic Benchmark for Evaluating Compliance in Multi-Agent Systems

## 基本資訊

- 發布日期：2026-06-10
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://arxiv.org/abs/2606.07805

## 概要

提出 MAC-Bench，首個動態對抗性基準，專門評估多代理系統在成功率與合規性產生權衡時的程序一致性。透過「世界建構者代理」生成高保真模擬環境（含資料庫延遲、API 錯誤碼、檔案權限等真實副作用），注入統一「合規憲章」涵蓋 GDPR、OWASP、MITRE ATT&CK、CIS 基準，在六大主流框架上測試，發現所有框架在壓力下均出現顯著合規違規，且違規率與任務成功率呈負相關。

## 核心價值

填補多代理評估「靜態基準無法捕捉對抗性合規壓力」的空白；證明 Goodhart 定律在代理系統中顯現——優化任務指標必然犧牲程序合規，需動態、對抗性基準持續監測。

## 應用情境與實務影響

企業部署多代理系統（金融審批、醫療決策、法務合規）可採用 MAC-Bench 持續審計；框架開發者（LangGraph、AutoGen、CrewAI、OpenAI SDK、Google ADK、MetaGPT）獲得標準化合規壓測流程；監管機構取得可量化的程序一致性指標。

## 補充細節

arXiv:2606.07805v1 (2026-06-10)。作者 Y. Zhao 等人。實驗涵蓋 LangGraph、AutoGen/AG2、CrewAI、OpenAI Agents SDK、Google ADK、MetaGPT 六大框架，配合 GPT-4o、Claude-3.5-Sonnet、Gemini-1.5-Pro、Qwen-2.5-72B 四模型。違規度量 Violation(τ) = Σ w_r·v_i,r / Σ w_r，權重依 CIS 基準嚴重度設定。

## 維護紀錄

- 收錄日期：2026-10-19
- 最後更新：2026-10-19

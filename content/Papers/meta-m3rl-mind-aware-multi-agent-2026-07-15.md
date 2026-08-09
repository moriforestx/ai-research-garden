---
title: "M3RL: Mind-Aware Multi-agent Management Reinforcement Learning"
type: paper
research_topic: "AI 代理人 / AI Agents"
published_date: "2026-07-15"
organization: "Meta AI"
source_url: "https://ai.meta.com/research/publications/m3rl-mind-aware-multi-agent-management-reinforcement-learning"
date_collected: "2026-08-10"
date_updated: "2026-08-10"
tags:
  - ai
  - paper
---

# M3RL: Mind-Aware Multi-agent Management Reinforcement Learning

## 基本資訊

- 發布日期：2026-07-15
- 研究主題：AI 代理人 / AI Agents
- 主要來源：https://ai.meta.com/research/publications/m3rl-mind-aware-multi-agent-management-reinforcement-learning

## 概要

Meta AI 於 2026 年 7 月 15 日發表 M3RL，���針對多智���慧體系統中工人智���慧體具有自主意���圖與���偏好（而非只服從命令）的場景，提出包含智���慧體建模與政策學���習的架構。透過線上建模工人智���慧體的心智（���偏好、意���圖、技能等），實現最���臨廣告組隊（ad-hoc teaming），在資源收集與製作兩個環境中���驗���證有效性。

## 核心價值

首次正式處理多智���慧體協作中的「智���慧體自主性」問題，而非假設所有智���慧體只會���盲目追求全域獎���勵；將理論����心智����建模����延伸至實際政策����學���習����，�������顯����提升在複�������雜、動態多智���慧體環境中的協調效能。

## 應用情境與實務影響

適用於需要考��慮人類或AI代理主觀意願的多代理系統：自動���駕���駛��������隊（不同車輛可能有不同優先����級）、智���慧製造（工作站有不同設定）、協同開發（開發者有不同專長）等場����境；提供建模與適應���異質性代理的通用���框架。

## 補充細節

方法：智���慧體建模����（線上推���斷工人����體的���偏好/意�圖/技能）+ 政策����學���習����（基於建模結果�������訓�������練管理者政策）。環境：資源收集（worker 有不同資源���偏好）與製作（worker 有不同製作技能/意���圖）。效能：在建模準確度與團隊獎���勵兩個維度上���顯著優於基線（���獨立 PPO/Q-learning 等）。開源：代理����與�������訓�������練食�������譜預計於 GitHub 發布。

## 維護紀錄

- 收錄日期：2026-08-10
- 最後更新：2026-08-10

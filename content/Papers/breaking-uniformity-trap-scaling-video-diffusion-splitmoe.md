---
title: "Breaking the Uniformity Trap: Scaling Video Diffusion Model via SplitMoE"
type: paper
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-29"
organization: "Sand.ai"
source_url: "https://arxiv.org/abs/2609.38140"
date_collected: "2026-10-02"
date_updated: "2026-10-02"
tags:
  - ai
  - paper
---

# Breaking the Uniformity Trap: Scaling Video Diffusion Model via SplitMoE

## 基本資訊

- 發布日期：2026-09-29
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2609.38140

## 概要

本文提出 SplitMoE 架構，解決擴展視頻擴散模型時的「均一性陷阱」問題。傳統 MoE 強制負載均衡導致路由不連貫、專家利用率不均。SplitMoE 採用原型引導路由與拉推正則化，讓 token 依語義屬性自然分群，區分特化專家與通用專家。在相同啟用參數預算下，SplitMoE 在收斂速度、路由連貫性與視頻生成品質上均優於傳統負載均衡 MoE。

## 核心價值

以語義驅動的原型路由取代強制負載均衡，實現視頻擴散模型的高效擴展，並在標準基準上達到 SOTA。

## 應用情境與實務影響

為大規模視頻生成模型提供可擴展的 MoE 架構範式；對文生視頻、視頻編輯等應用具有直接價值。

## 補充細節

arXiv:2609.38140v1 [cs.CV]，提交日期 2026-09-29。已獲 NeurIPS 2026 Spotlight 接受。作者：Yu Xu 等 10 位研究者，隸屬 Sand.ai。

## 維護紀錄

- 收錄日期：2026-10-02
- 最後更新：2026-10-02

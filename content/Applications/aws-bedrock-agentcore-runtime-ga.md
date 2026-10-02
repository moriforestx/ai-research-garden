---
title: "AWS 發布 Bedrock AgentCore Runtime GA：受管代理執行環境支援 14 天長程會話"
type: application
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-09-18"
organization: "Amazon Web Services"
source_url: "https://aws.amazon.com/about-aws/whats-new/2026/09/new-agentcore-runtime-generally-available"
date_collected: "2026-10-03"
date_updated: "2026-10-03"
tags:
  - ai
  - application
---

# AWS 發布 Bedrock AgentCore Runtime GA：受管代理執行環境支援 14 天長程會話

## 基本資訊

- 發布日期：2026-09-18
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://aws.amazon.com/about-aws/whats-new/2026/09/new-agentcore-runtime-generally-available

## 概要

AWS 於 2026 年 9 月 18 日宣佈 Amazon Bedrock AgentCore Runtime 正式達到 GA（正式版）。AgentCore Runtime 為受管運算層，提供專用、持久的代理執行實例，取代共享暫時性執行；會話最長可維持 14 天，解決長程代理的狀態管理難題。同步支援代理框架評估、TypeScript 框架（Strands Agents、LangGraph、OpenAI Agents、Vercel AI SDK）、CDK L2 Constructs 穩定版、MCP Gateway、Identity、Code Interpreter、Browser 等模組化服務。原 Bedrock Agents 於 7 月初移至維護模式（Bedrock Agents Classic），新開發建議遷移至 AgentCore。

## 核心價值

首個雲原生、企業級受管代理執行層，原生支援長程會話與框架無關部署

## 應用情境與實務影響

企業可在無 DevOps 負擔下部署生產級多代理系統；IAM 主體級成本歸因支援 FinOps 精細核算

## 補充細節

AgentCore 於 2026 年分階段發布：3 月 Policy GA、5 月 CDK Constructs 穩定、7 月 MCP Gateway 更新、8 月 DynamoDB 原生向量搜尋 GA、9 月 Runtime GA。官方部落格技術深度文：https://aws.amazon.com/blogs/machine-learning/the-new-agentcore-runtime-elastic-optimized-and-consistently-fast-starts。

## 維護紀錄

- 收錄日期：2026-10-03
- 最後更新：2026-10-03

---
title: "AWS 連續發布 DynamoDB 原生向量搜尋 GA、Bedrock AgentCore 執行環境 GA 與 Web Search，完善代理式 AI 基礎設施"
type: technical-development
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-08-05"
organization: "Amazon Web Services"
source_url: "https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-dynamodb-vector-search"
date_collected: "2026-10-01"
date_updated: "2026-10-01"
tags:
  - ai
  - technical-development
---

# AWS 連續發布 DynamoDB 原生向量搜尋 GA、Bedrock AgentCore 執行環境 GA 與 Web Search，完善代理式 AI 基礎設施

## 基本資訊

- 發布日期：2026-08-05
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-dynamodb-vector-search

## 概要

AWS 於 2026 年 8 月第一週密集推出三項生產級代理基礎設施：(1) 8/5 DynamoDB 原生向量搜尋正式上線（GA），支援單一項目內嵌入向量屬性、SearchVectors API、餘弦/歐氏距離/內積三種距離函數、最高 4096 維、單位毫秒級延遲 99%+ 召回率、支援萬億級向量；(2) 8/10 Bedrock AgentCore 執行執行個體 GA，提供專用代理執行環境、可預測效能與成本；(3) Bedrock 內建 Web Search（GA），代理可直接檢索即時公開網頁資訊。同期另宣佈 Agent Plugins 開放標準，支援 Kiro、VS Code、Cursor 等跨工具可攜式代理擴充。

## 核心價值

將向量檢索下沉至營運資料庫（DynamoDB），消除獨立向量資料庫架構複雜度；AgentCore 提供受管代理運行時，降低自建基礎設施門檻；三項功能同步上線形成完整代理部署鏈路。

## 應用情境與實務影響

企業可在既有 DynamoDB 表直接啟用語義檢索，無需遷移資料或運維第二資料庫；AgentCore 適合需嚴格隔離、合規或成本可控的代理工作負載；Web Search 解決代理知識截止問題；Agent Plugins 標準促進生態互通。

## 補充細節

DynamoDB 向量搜尋：全商業區域 + GovCloud 上線，項目大小限制 400 KB 不變。AgentCore：Sébastien Stormacq 部落文說明用法。Web Search：6/19 預覽、8 月 GA。官方來源：AWS What's New (DynamoDB)、AWS News Blog (Weekly Roundup Aug 10)、Bedrock AgentCore 文件。

## 維護紀錄

- 收錄日期：2026-10-01
- 最後更新：2026-10-01

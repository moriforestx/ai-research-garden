---
title: "Amazon Bedrock AgentCore Runtime Instances：面向生產級 AI 代理的持久託管 EC2 基礎設施正式上線"
type: technical-development
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-08-10"
organization: "Amazon Web Services"
source_url: "https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore"
date_collected: "2026-11-03"
date_updated: "2026-11-03"
tags:
  - ai
  - technical-development
---

# Amazon Bedrock AgentCore Runtime Instances：面向生產級 AI 代理的持久託管 EC2 基礎設施正式上線

## 基本資訊

- 發布日期：2026-08-10
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore

## 概要

AWS 正式發布 Amazon Bedrock AgentCore Runtime Instances，為生產級 AI 代理提供持久、託管的 EC2 基礎設施。相較於預設的微型 VM（會話 ≤8 小時、快速啟動），Runtime Instances 支援長達 14 天的長期會話、GPU 加速、多代理共置協作、會話停止/重啟省成本、容器化部署，並可選用完整 EC2 執行個體類型（GPU、記憶體優化、運算優化）。同步上線 AWS Agent Registry（自動偵測、客戶管理金鑰加密）與 DynamoDB 原生向量搜尋。已在 9 個區域 GA。

## 核心價值

將代理運行時從「暫時性無狀態」提升為「持久有狀態、可攜帶專屬依賴與硬體」，解決長時間運行、重運算、多代理協作的生產部署缺口。

## 應用情境與實務影響

適用於程式碼編譯/安全掃描/資料管線等長時間運算代理、需共享記憶體的多代理編排、GPU 密集型推理工作負載。團隊可透過 Capacity Provider 宣告所需 EC2 型別，透過相同 AgentCore API 無縫切換微型 VM 與 Instances。

## 補充細節

AWS News Blog 發布於 2026-08-10（對應 What's New 公告 2026/08）。Release Notes 確認 2026-08 月份新增「Runtime instances」GA 項目。同期 8/5 釋出 DynamoDB 向量搜尋 GA、8/10 釋出 AgentCore Runtime Instances GA、8/19 釋出 Web Search 連接器 GA。定價包含管理費 + 底層 EC2 費用。支援區域：US East (N. Virginia/Ohio)、US West (Oregon)、APAC (Mumbai/Singapore/Sydney/Tokyo)、EU (Frankfurt/Ireland)。

## 維護紀錄

- 收錄日期：2026-11-03
- 最後更新：2026-11-03

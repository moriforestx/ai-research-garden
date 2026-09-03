---
title: "AWS expands G7e Blackwell GPU instances to SageMaker AI inference in Asia and Europe for enhanced LLM deployment performance"
type: technical-development
research_topic: "AI 應用與部署 / AI Applications & Deployment"
published_date: "2026-07-01"
organization: "AWS"
source_url: "https://aws.amazon.com/about-aws/whats-new/2026/07/g7e-sagemaker-ai"
date_collected: "2026-09-04"
date_updated: "2026-09-04"
tags:
  - ai
  - technical-development
---

# AWS expands G7e Blackwell GPU instances to SageMaker AI inference in Asia and Europe for enhanced LLM deployment performance

## 基本資訊

- 發布日期：2026-07-01
- 研究主題：AI 應用與部署 / AI Applications & Deployment
- 主要來源：https://aws.amazon.com/about-aws/whats-new/2026/07/g7e-sagemaker-ai

## 概要

AWS 在 2026 年 7 月 1 日宣布在亞太首爾、歐洲倫敦和亞太東京三個新區域提供 Amazon EC2 G7e 執行個體用於 Amazon SageMaker AI 推理服務。這些實例搭載最多 8 顆 NVIDIA RTX PRO 6000 Blackwell Server Edition GPU，每顆提供 96 GB 記憶體，總計可達 768 GB GPU 記憶體，使單一實例能夠以 FP8 精度運行多達 70B 參數的大型語言模型，無需多節點配置。相比舊一代 G6e 實例，推理效能提升最高達 2.3 倍，同時提供最高 1,600 Gbps 的彈性網路介面卡頻寬。

## 核心價值

新一代 Blackwell 架構 GPU 實例在 SageMaker 上的區域擴張，顯著提升大型語言模型推理效能並降低延遲。

## 應用情境與實務影響

企業現在可以在靠近亞洲和歐洲終端用戶的位置部署更大型的語言模型，減少網路延遲並提升使用者體驗，特別適合需要即時回應的生成式 AI 應用程式，如聊天機器人、虛擬助理和內容生成系統。

## 補充細節

G7e 實例特色包括：每顆 NVIDIA RTX PRO 6000 Blackwell Server Edition GPU 提供 96 GB HBM3E 記憶體；第五代 Intel Xeon 處理器；最高 1,600 Gbps 的 Elastic Fabric Adapter (EFA) 網路頻寬；支援 NVIDIA GPUDirect P2P 和 RDMA 以加速多 GPU 工作負載。這些實例特別適合 LLM 推理、圖像與視訊生成、空間運算及科學計算工作負載。區域擴張意味著客戶現在可以將推理端點部署在亞太首爾、歐洲倫敦和亞太東京（加上先前已支援的區域），讓他們能夠將模型部署得更靠近終端用戶基礎設施，從而減少傳輸延遲並提升互動式 AI 應用程式的回應速度。

## 維護紀錄

- 收錄日期：2026-09-04
- 最後更新：2026-09-04

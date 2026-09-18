---
title: "Open ultrasound foundation model for robust segmentation and clinical measurement across heterogeneous settings"
type: tool
research_topic: "電腦視覺 / Computer Vision"
published_date: "2026-09-18"
organization: "Chao Qin, Fahad Shahbaz Khan, Salman Khan, Sarim Ather, Siddiq Anwar, Rao Muhammad Anwer, Shadab Khan"
source_url: "https://arxiv.org/abs/2609.19230"
date_collected: "2026-09-19"
date_updated: "2026-09-19"
tags:
  - ai
  - tool
---

# Open ultrasound foundation model for robust segmentation and clinical measurement across heterogeneous settings

## 基本資訊

- 發布日期：2026-09-18
- 研究主題：電腦視覺 / Computer Vision
- 主要來源：https://arxiv.org/abs/2609.19230

## 概要

提出 SonoCorpus（開放資源，統一來自 53 個公開資料集的 456,963 張影像和 1,626,085 個專家遮罩，橫跨 24 個臨床應用和 17 個國家）和 SonoBase（在其上預訓練的互動式分割基礎模型）。在十五個引入新器官、設備、操作者和地理位置的評估資料集上，SonoBase 在每個資料集上均優於 SAM2、MedSAM2 和可提示 MedSAM3；在完全外部資料上，其表現超越這些基準模型在其自身分佈基準上的表現。

## 核心價值

提供一個強大且通用的超聲波 AI 基礎模型，能夠在不同設備、操作者和解剖結構的環境中穩定工作，減少對特定場景的重新訓練需求。

## 應用情境與實務影響

使超聲波 AI 在真實臨床環境中的部署變得更加可行，特別是在資源有限的地區（如塞拉利昂和坦尚尼亞），只需五個標註範例即可適應新環境。

## 補充細節

SonoBase 在推斷心臟射出分數時的誤差為 6.63%（落在觀察者間變異範圍內），在除額外細胞激勵器候選門檻的誤判率為 13%，優於基準模型的 18--42%。胎兒頭圍誤差為 1.81 mm，妊娠週期誤差為 1.2 天，兩者均低於觀察者間變異。在基線模型完全失敗的一半測試案例中，SonoBase 能在 81% 的情況下恢復可用的分割結果。釋出所有檢查點、優化器狀態、資料分割索斷、去重雜湊和入門程式碼，確保可重複性並促進社區建構。

## 維護紀錄

- 收錄日期：2026-09-19
- 最後更新：2026-09-19

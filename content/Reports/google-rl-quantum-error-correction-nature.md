---
title: "Towards a quantum computer that learns from its errors"
type: report
research_topic: "AI 綜合動態 / General AI Updates"
published_date: "2026-07-22"
organization: "Google Research / Google DeepMind"
source_url: "https://research.google/blog/towards-a-quantum-computer-that-learns-from-its-errors"
date_collected: "2026-07-27"
date_updated: "2026-07-27"
tags:
  - ai
  - report
---

# Towards a quantum computer that learns from its errors

## 基本資訊

- 發布日期：2026-07-22
- 研究主題：AI 綜合動態 / General AI Updates
- 主要來源：https://research.google/blog/towards-a-quantum-computer-that-learns-from-its-errors

## 概要

Google Research 於 2026 年 7 月 22 日發布技術部落格，宣佈在《Nature》發表《Reinforcement learning control of quantum error correction》。研究展示以強化學習（RL）代理人從量子錯誤偵測事件中學習，在線調控超導量子處理器 Willow 的數千個控制參數，於計算過程中持續校準、抵抗漂移。實驗證明：在刻意注入人工漂移條件下，RL 導向使表面碼邏輯穩定性提升 3.5 倍；即使經專家級人工精調後，RL 微調仍能再降 20% 邏輯錯誤率。綜合所有技術後，表面碼邏輯錯誤率降至每千次錯誤校正週期 <1 次、色碼 <1 次/百次。模擬顯示 RL 訓練週期與系統規模無關，展示可擴展性。此成果開啟「量子電腦從錯誤中學習且不停機」的新範式。

## 核心價值

首次在實體量子硬體上證明 RL 代理人可利用 QEC 偵測事件作為即時學習信號，在線持續校準控制參數，打破「計算與校準必須分離」的長期瓶頸，為容錯量子運算邁出關鍵一步。

## 應用情境與實務影響

量子硬體團隊可直接採用此 RL 框架縮減人工校準工時，並與既有 AlphaQubit、Tesseract 解碼器串接；隨著量子位數擴展，RL 訓練樣本效率不隨規模下降，利於大規模容錯機器部署。

## 補充細節

對應論文：Reinforcement learning control of quantum error correction (Nature, 2026-07-22, DOI: 10.1038/s41586-026-10759-2)。作者團隊：Google Quantum AI（Google Research）與 Google DeepMind 合作。實驗在 Willow 超導處理器（105 量子位）執行；RL 代理人採 PPO，觀測空間為 QEC 檢測事件歷史，動作空間為控制參數微調。代碼與數據將配合論文發布。

## 維護紀錄

- 收錄日期：2026-07-27
- 最後更新：2026-07-27

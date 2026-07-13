---
title: "F5E-TTS: Enhancing Speech Synthesis by Aligning Text with Rich Semantic Representations"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-05-01"
authors:
  - "Yihang Chen"
  - "Hualei Wang"
  - "Na Li"
  - "Zhifeng Li"
keywords:
  - "speech synthesis"
  - "semantic alignment"
  - "TTS"
  - "prosody modeling"
  - "ICASSP 2026"
identifier: "ICASSP2026-F5E-TTS"
identifier_type: "conference"
publication_status: "published"
source_url: "https://2026.ieeeicassp.org/industry_program"
date_collected: "2026-07-13"
date_updated: "2026-07-13"
tags:
  - ai
  - paper
---

# F5E-TTS: Enhancing Speech Synthesis by Aligning Text with Rich Semantic Representations

## 基本資訊

- 作者：Yihang Chen、Hualei Wang、Na Li、Zhifeng Li
- 發布日期：2026-05-01 (ICASSP 2026)
- 研究主題：音訊與語音 / Audio & Speech
- 關鍵字：speech synthesis、semantic alignment、TTS、prosody modeling、ICASSP 2026
- 論文識別碼：ICASSP2026-F5E-TTS (conference)
- 發表狀態：已發表
- 主要來源：https://2026.ieeeicassp.org/industry_program

## 摘要

提出 F5E-TTS，透過將文本與豐富語義表示對齊來增強語音合成。結合文本編碼器與語義編碼器，捕捉韻律、情感、說話人特徵等超段屬性，顯著提升合成語音的自然度與表現力。

## 核心研究問題

如何在 TTS 架構中有效融入豐富語義資訊，解決傳統 TTS 忽略超段屬性導致合成語音平淡的問題？

## 方法與技術

雙編碼器架構：文本編碼器提取語言內容，語義編碼器從參考音頻或文本上下文提取韻律、情感、說話人身份等超段語義。透過對齊模組將兩路表示融合，送入聲學模型生成梅爾頻譜，再由聲碼器合成波形。

## 實驗與研究結果

在多語言、多說話人基準上，主觀 MOS 與客觀指標（WER、SIM、PESQ）均顯著優於 FastSpeech 2、VITS 等基線。消融實驗證實語義對齊模組對表現力提升貢獻最大。

## 研究意義與適用範圍

推進語義感知 TTS 架構，適用於有聲書、虛擬助理、客服語音、內容創作等需高表現力語音合成場景。

## 限制與注意事項

需參考音頻或上下文提供語義條件；零樣本情境下語義編碼器泛化性待驗證。

## 相關概念

- 語音合成
- 韻律建模
- 語義對齊
- 零樣本 TTS

## 相關工具與專案

- ICASSP 2026 開放獲取版本

## 維護紀錄

- 收錄日期：2026-07-13
- 最後更新：2026-07-13
- 更新紀錄：
  - 2026-07-13：首次建立

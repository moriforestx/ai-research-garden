---
title: "ISCSLP 2026 CoT-TTS Challenge：引入鏈式思維推理的語境感知語音合成基準"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-21"
organization: "ISCSLP 2026 / Nanjing University / HKUST"
source_url: "https://arxiv.org/abs/2606.21933"
date_collected: "2026-10-22"
date_updated: "2026-10-22"
tags:
  - ai
  - paper
---

# ISCSLP 2026 CoT-TTS Challenge：引入鏈式思維推理的語境感知語音合成基準

## 基本資訊

- 發布日期：2026-06-21
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2606.21933

## 概要

ISCSLP 2026 會議推出 CoT-TTS Challenge，首次將鏈式思維（Chain-of-Thought）推理引入語境感知文字轉語音（TTS）任務。挑戰要求模型在生成語音前，先以 CoT 形式推理語境適配的韻律、情感與說話風格，再合成波形。基準包含多語言、多場景測試集，評估指標涵蓋自然度、語境一致性與風格準確度。來自南京大學、港科大等機構的研究者共同組織，旨在推動 TTS 從「朗讀」邁向「理解後表達」。

## 核心價值

建立首個以 CoT 結構化推理為核心的 TTS 基準，重新定義語境感知語音合成的評估維度，推動語音模型向多模態推理邁進。

## 應用情境與實務影響

為 TTS 系統引入可解釋的推理階段，便於診斷韻律/情感錯誤來源；基準開源可直接用於模型選型與改進，適用於有聲書、虛擬助手、客服機器人等需語境適配的場景。

## 補充細節

論文編號：arXiv:2606.21933v1 (eess.AS; cs.CL; cs.SD)，2026-06-21 提交。主辦單位：ISCSLP 2026（International Symposium on Chinese Spoken Language Processing）。核心設計：(1) 兩階段流程——CoT 推理階段輸出結構化推理鏈，合成階段條件化生成；(2) 涵蓋中英日韓等多語言、敘事/對話/廣播等場景；(3) 採用 BiCodec 音頻編碼與 Qwen3 分詞器統一文本/音頻表示；(4) 釋出訓練數據、評估腳本與排行榜。相關機構：南京大學、香港科技大學。

## 維護紀錄

- 收錄日期：2026-10-22
- 最後更新：2026-10-22

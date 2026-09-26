---
title: "TLDR: Compressing Audio Tokens for Efficient Autoregressive Text-to-Speech"
type: paper
research_topic: "音訊與語音 / Audio & Speech"
published_date: "2026-06-08"
organization: "Sungkyunkwan University / University of Seoul"
source_url: "https://arxiv.org/abs/2606.09019"
date_collected: "2026-09-27"
date_updated: "2026-09-27"
tags:
  - ai
  - paper
---

# TLDR: Compressing Audio Tokens for Efficient Autoregressive Text-to-Speech

## 基本資訊

- 發布日期：2026-06-08
- 研究主題：音訊與語音 / Audio & Speech
- 主要來源：https://arxiv.org/abs/2606.09019

## 概要

Sungkyunkwan University 與 University of Seoul 研究團隊提出 TLDR，一種基於補丁的自回歸 TTS 框架，將 codec-based AR-TTS 的建模單位從單一音訊 token 升級為 token patches，大幅降低推理成本。核心創新：(1) Token-to-Patch Compressor 將連續 codec tokens 壓縮為緊湛的潛在補丁表示；(2) 凍結預訓練 AR-TTS backbone（CosyVoice3），僅用 LoRA 適配器調整至補丁層級建模；(3) Speaker-Conditioned Patch-to-Token Extractor 在各補丁內局部自回歸生成細粒度 tokens，保留說話人特徵。實驗顯示：patch size k=4 時，全域 backbone KV-cache 記憶體降低 75%，推理速度提升 1.8x，零樣本 TTS 的 WER 與說話人相似度 (SIM) 僅輕微下降。證明補丁層級全域因果建模是降低 AR-TTS 推理成本的實用路徑，無需替換既有 tokenizer、前端與 vocoder。

## 核心價值

為 codec-based AR-TTS 提供即插即用的加速方案：在不重新訓練龐大 backbone 前提下，透過補丁層級重構實現記憶體與延雙重優化，直接適用於 VALL-E、CosyVoice、Seed-TTS、LLaSA 等主流零樣本 TTS 系統。

## 應用情境與實務影響

降低即時語音合成、聲音轉換、多語言 TTS 部署門檻；對邊緣裝置語音助手、即時翻譯、無障礙輔助技術具高價值。LoRA 適配策略使現有模型可低成本遷移。

## 補充細節

arXiv:2606.09019v1 [cs.SD]，提交日期 2026-06-08。作者：Yejin Lee、Junwon Moon、Hyoeun Kim、Hyunjin Choi、Heeseung Kim、Kyuhong Shim (Sungkyunkwan Univ. / Univ. of Seoul)。使用 CosyVoice3 作為 backbone，SeedTTS-EN 測試集評估。License: CC BY-NC-ND 4.0。屬 Audio & Speech 核心技術研究。

## 維護紀錄

- 收錄日期：2026-09-27
- 最後更新：2026-09-27

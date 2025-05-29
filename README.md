# NYCU ICLAB 2023 Fall 修課指南 - TA 心得紀錄

## 🧭 Overview

歡迎來到 ICLAB 2023 Fall 的非官方 TA 修課指南！

這份筆記由我整理，身為多屆 ICLAB 大助教，這是根據實際帶課經驗與觀察到的學生常見痛點所撰寫。我希望這不只是課程筆記，而是一份真正能幫助你理解設計思路、學會高效實作、少走冤枉路的學習資源。

這堂課不只考驗技術，也挑戰心理素質。如果你正努力通過這場修課洗禮，這份指南就是為你準備的。

> **TA 經歷：**  
> ICLAB 大助教：2023 Fall, 2021 Fall  
> ICLAB 小助教：2021 Spring  
> VLSI Lab 大助教：2022 Fall  
> Intro. to VLSI：2022 Fall

我也曾經是這門課的學生，走過一樣的迷惘、通宵、焦慮與成就感。這些經驗讓我希望 ICLAB 不只是「交作業」的地方，而是一個讓你真正學會如何設計出高效、穩定、能在職場中發揮價值的電路。

如果多年後你能回頭感謝這堂課，那就值得了。

覺得這份筆記對你有幫助嗎？歡迎在 GitHub 上點個 Star ⭐️，讓更多人看到這份資源！

[![GitHub Stars](https://img.shields.io/github/stars/lhlaib/NYCU-ICLAB-2023-Fall.svg?style=social)](https://github.com/lhlaib/NYCU-ICLAB-2023-Fall) [![GitHub Follow](https://img.shields.io/github/followers/lhlaib?label=Follow&style=social)](https://github.com/lhlaib)


## 📚 目錄

#### 1️⃣ 認識這門課
- [🧭 Overview](#-overview)
- [📘 課程介紹](#-課程介紹)
- [✍️ 前言：TA 的觀察與建議](#-前言-ta-的觀察與建議)
- [🔠 課程內容（Lecture 一覽）](#-課程內容lecture-一覽)
- [🧪 實驗總覽（Lab 一覽與難度）](#-實驗總覽lab-一覽與難度)

#### 2️⃣ 修課前的準備
- [🎯 背景與修課建議](#-背景與修課建議)
- [🔧 修課前技能樹 Checklist](#-修課前技能樹-checklist)

#### 3️⃣ 修課進行時
- [📂 各 Lab 設計思路與驗證技巧（待補）](#-各-lab-設計思路與驗證技巧待補)
- [🧰 推薦工具：驗證自動化 / Debug 技巧 / Pattern Generator](#-推薦工具驗證自動化--debug-技巧--pattern-generator)

#### 4️⃣ 心態經營與生存法則
- [🧠 TA 的修課心法與提醒](#-ta-的修課心法與提醒)
- [❓ 常見問題 FAQ](#-常見問題-faq)
- [📦 補充資源與外部連結](#-補充資源與外部連結)

---



## 📘 課程介紹

本課程旨在教導高年級及碩士班之電子工程學生使用最先進 CAD 工具設計 VLSI 晶片的技術。從 RTL 架構設計、Verilog HDL 開發、測試驗證、Synthesis、APR 到最終的 GDSII，都會在這 18 週中完整體驗。課程核心包含：

- Top-down IC 設計流程
- Verilog/SystemVerilog 開發與模擬
- 靜態時序分析（STA）與 Formal Verification
- Power/Performance/Area (PPA) 優化實作

實驗與專題則以設計挑戰為導向，考驗同學從規格解讀、模組劃分、驗證到效能分析的整合能力。

課程評分多以 RANK 評比、驗證正確性與 PPA 為主，競爭激烈。

---

## ✍️ 前言

作為這門課的助教與學長，我常常見證學生從信心滿滿到迷惘、懊惱、再到成長蛻變的整個過程。這門課不是傳統的作業打卡課，而是你能否「快速學會做對事」與「在有限時間內交付品質」的真實演練場。

修完這門課的你，不一定會立刻變成 RTL 專家，但一定會對 IC 設計的複雜性、架構思維與驗證流程有深刻體會。

這份學習指引，除了技巧與設計，也希望能為你的心態與節奏提供一份實用的參考。

---

## 🔠 課程內容

| Lecture | Topic |
|:--|:--:|
|Lecture01|Cell Based Design Methodology + Verilog Combinational Circuit Programming|
|Lecture02|Finite State Machine + Verilog Sequential Circuit Programming |
|Lecture03|Verification & Simulation + Verilog Test Bench Programming |
|Lecture04|Sequential Circuit Design II (STA + Pipeline) |
|Lecture05|Memory & Coding Style (Memory Compiler + SuperLint)|
|Lecture06|Synthesis Methodology (Design Compiler + IP Design)|
|Lecture07|Timing: Cross Clock Domain + Synthesis Static Time Analysis|
|Lecture08|System Verilog - RTL Design|
|Lecture09|System Verilog - Verification|
|Lecture10|System Verilog - Formal Verification|
|Lecture11|Power Analysis & Low Power Design|
|Lecture12|APR I : From RTL to GDSII|
|Lecture13|APR II: IR-Drop Analysis|

---

## 🧪 實驗總覽

| Lab | Topic | RANK | Pass Rate |
|:--|:--:|:--:|:--:|
|[Lab01](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab01_iclab065>)|Code Calculator|21|89.76%|
|[Lab02](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab02_iclab065>)|Enigma Machine|16|85.83%|
|[Lab03](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab03_iclab065>)|AXI-SPI DataBridge|NA|75.59%|
|[Lab04](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab04_iclab065>)|Convolution Neural Network|22|74.80%|
|[Lab05](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab05_iclab065>)|Matrix convolution, max pooling and transposed convolution|15|59.06%|
|[Lab06](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab06_iclab065>)|Huffman Code Operation|60|77.95%|
|[Lab07](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab07_iclab065>)|Matrix Multiplication with Clock Domain Crossing|58|74.80%|
|[Lab08](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab08_iclab065>)|Design: Tea House|NA|66.14%|
|[Lab09](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab09_iclab065>)|Verification: Tea House|1|66.14%|
|[Lab10](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab10_iclab065>)|Formal Verification|NA|76.38%|
|[Lab11](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab11_iclab065>)|Low power design: Siamese Neural Network|4|67.72%|
|[Lab12](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab12_iclab065>)|APR: Matrix convolution, max pooling and transposed convolution|3|68.50%|
|[Lab13](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Lab13_iclab065>)|Train Tour APRII|NA|68.50%|
|[Online Test](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/OT_iclab065>)|Infix to prefix convertor and prefix evaluation|NA|2.36%|
|[Midtern Project](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Midterm_Project_iclab065>)|Maze Router Accelerator|53|68.50%|
|[Final Project](<https://github.com/kevin861222/NYCU-ICLAB-2024-Spring/tree/main/Mycode/Final_Project>)|single core CPU|3|67.72%|

---

## 🎯 背景

### 修課前技能樹

- ✅ 熟悉 Verilog RTL 撰寫
- ✅ 略懂 SystemVerilog（SV 僅佔 1-2 個 Lab）
- ✅ 熟悉 Python，能撰寫 pattern generator
- ✅ 基礎 shell script：加速驗證流程極佳利器
- ✅ 基礎 Linux 操作：Server 上傳下載、排程執行等
- ✅ 使用 tmux / nohup / screen 進行後台作業管理
- ✅ 若能補完 HDLBits、看過張添烜教授數位系統設計影片，更佳

這些能力不需要在開學前就全會，但能提早準備就能更快進入狀況，也會讓你在 Lab5～Lab6 的高峰期喘得沒那麼辛苦。





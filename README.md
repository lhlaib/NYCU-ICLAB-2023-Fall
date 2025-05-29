
# NYCU ICLAB 2023 Fall 修課指南 from TA Perspective


## 🧭 Overview

歡迎來到 ICLAB 2023 Fall 的非官方 TA 學習指南！
這是一份由曾擔任多屆課程大助教所整理的實戰經驗精華，根據自身的協助經驗、觀察學生常見問題與痛點所整理，目的在於提供一份比「僅有課程筆記」更有深度的修課輔助資源。
希望幫助每一位認真修課的你，在這場硬實力與心理素質並重的課程裡，更有效率地學習、少走冤枉路。

> **TA 經歷：**  
> ICLAB 大助教：2023 Fall, 2021 Fall  
> ICLAB 小助教：2021 Spring  
> VLSI Lab 大助教：2022 Fall  
> Intro. to VLSI：2022 Fall


我曾經是修課的學生，也曾見證過超過 300 位學生走過這門課程的歷程。這份心得是經年累月所累積的教學與陪伴的結晶。我希望iclab這門課不只是個「交作業的地方」，更是幫助你理解設計背後的思考脈絡與實作技巧、學會如何寫出一個高效能且可維護的電路、甚至是未來踏入職場時，回頭感謝這堂課的起點之一。


## 目錄
1. [摘要](#摘要)
2. [課程介紹](#課程介紹)
3. [前言](#前言)
4. [背景](#背景)
5. [主觀聲明](#主觀聲明)



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





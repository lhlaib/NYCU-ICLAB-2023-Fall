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

## 1️⃣ 認識這門課

### 📘 課程介紹

本課程目標在教導研究所/大學部學生使用最先進 CAD 工具設計 ASIC/VLSI 晶片的技術。從 RTL 架構設計、Verilog HDL 開發、測試驗證、Synthesis、APR 到最終的 GDSII，都會在這 18 週中完整體驗。課程核心包含：

- Verilog 語法：RTL 設計、FSM 與 Coding Style
- 設計驗證： Simulation、Formal Check, 熟悉 Pattern/Assertion Based Verification
- 數位設計流程：Cell-based Design Flow, Synthesis、APR（從 RTL 到 GDS）
- 進階設計技巧：STA、IR-Drop、Cross Clock Domain, Low Power Design

特色：

- 一學期內熟悉使用業界標竿工具（DC, VCS, Verdi, Jasper, Innovus, ...）
- 實作 UMC 0.18 製程 與 TSMC 16 nm FinFET 製程 並比較先進製程性能
- 所有 Lab 都有 PPA 評分與排名（RANK），模擬真實業界競爭環境
- 13 個 Labs + 2 個 Projects + 2 個 Exams + 1 個 Online Test = 魔鬼訓練

這門課會讓你學到：

- 如何建構一個結構化的數位系統架構（不只是寫 code）
- 如何面對週週交作業、交 project 的壓力，培養時間管理與抗壓能力
- 如何 Debug，如何查 datasheet，如何靠自己解決沒有標準解答的問題

你也會體會到：

- 壓力來臨時要選擇「妥協還是堅持」
- 錯過 Deadline，功能錯誤，就是0，沒有藉口
- 成績不等於實力，但過程累積的實力，才是你的競爭力
- 這門課的成績，絕對不是你學習的全部，但它會讓你更清楚自己的不足與未來的方向


### ✍️ 前言

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

## 2️⃣ 修課前的準備


### 🎯 背景與修課建議

許多學生進入 ICLAB 前會問：「我需要多會 Verilog 才能修這門課？」但事實上，Verilog 的熟練程度並不是你能否撐過這門課的關鍵。

這門課真正要求的，是你能否：

- **理解整體設計流程**：從 RTL 架構到實體實現，不只是會寫 Code，而是能做決策。
- **獨立面對問題**：尤其是在壓力之下 debug 與查找資源的能力。
- **建立良好習慣**：從 file 結構管理、驗證邏輯、編譯腳本，到 version control。

#### 建議修課前具備：

- 至少修過一門 Verilog/RTL 課程（如：數位電路、系統晶片設計）
- 熟悉基本的 Linux 指令（cd、vim、scp、screen/tmux 等）
- 熟悉 Python（生成 pattern、驗證用）
- 有「試圖寫出乾淨架構」的意願


### 🔧 修課前技能樹 Checklist

以下是 TA 建議的技能地圖（越早準備越有利）：

- ✅ 熟悉基本 Verilog 語法與 FSM 架構
- ✅ 熟悉常見電路模組（加減乘除、Decoder、MUX、FIFO、SRAM 控制器等）
- ✅ 熟悉 Python（簡單的字串處理、檔案讀寫、陣列操作）
- ✅ 熟悉 shell script 或 Makefile
- ✅ 熟悉 git 的基本操作（clone / commit / diff / push）
- ✅ 知道如何使用 Waveform Viewer（DVE、GTKWave）
- ✅ HDLBits 練習題目完成 80% 以上（https://hdlbits.01xz.net/）

> 🌱 技術以外，更重要的是「面對錯誤時的態度」。懂得整理錯誤訊息、一步步排查，是這門課最珍貴的軟實力。


## 3️⃣ 修課進行時

### 🛠 面對問題，助教建議這樣做：
##### ✅ 1. 積極與同學討論

- 「為什麼這個 Bug 出現？」
- 「為什麼 03 Violation？是哪個控制訊號沒有回來？」
- **懂得問問題，遠比自己卡住 10 小時有價值**

##### ✅ 2. 善用網路資源

- [VLSIbits](https://vlsibits.net/)：設計風格與技巧講解
- GitHub 搜尋 `iclab`、`axi spi`、`cnn verilog`，站在巨人的肩膀上吸收架構與概念
- HackMD 或學長姐部落格：很多人記錄過實戰心得

##### ✅ 3. 明智使用 AI / GPT

AI 是雙面刃。**用得好，如虎添翼；用錯了，一事無成。**

你可以：

- 使用 GPT 幫你釐清設計邏輯、整理 testbench 的檢查點
- 幫你整理 RTL module 的撰寫順序與命名風格
- 用 Copilot 自動補充重複性語法、流水線 template

但請**千萬不要**：

- 直接請 GPT 改寫前人 code
- 輸入題目描述請 GPT 寫完整的 module

> 你不只是在學寫語法，你是在學如何設計與架構邏輯系統。這是精髓。

##### ✅ 4. 找助教問對的問題

助教不只是批改作業的角色，我們其實非常希望：

- 有人來問：「這樣寫會不會有架構問題？」
- 有人來說：「這段我實在不懂，能幫我解釋嗎？」
- 有人誠實說：「我不知道這題該從哪裡下手」

助教不會給你答案，但會**幫你釐清盲點、確認你設計的思路是不是穩的**。


### 4️⃣ 心態經營與生存法則


---

## 📂 各 Lab 設計思路與驗證技巧（持續撰寫中）

### Lab01 - Code Calculator

- FSM 設計的熱身題，重點在於理解 finite state control 的結構劃分。
- 雖然題目簡單，但仍可從：
  - 如何模組化 Input Decoder
  - 如何管理狀態轉移與有效訊號
  - 如何規劃 Testbench 驗證輸入序列
  取得穩定高分。

---

### Lab02 - Enigma Machine

- 加密邏輯與資料流控制的第一個挑戰。
- 特別容易漏驗 corner case，建議：
  - 將 pattern 分類整理，補上不同組合測試
  - 嚴格對照 spec 與 TA 給的注意事項

---

### Lab03 - AXI to SPI DataBridge

- 進入 Cross-Domain 與 Protocol Interface 設計
- 推薦策略：
  - 抽象化 Address Decoder 與 FSM
  - 使用 FIFO 或 Double Buffer 解決 Timing 不一致
  - 把 Write、Read、SPI 等模組獨立分開處理

---

> 🔍 每個 Lab 的挑戰都不是「單一模組」的設計，而是系統性的思考與測試策略規劃。

---

## 🧰 推薦工具：驗證自動化 / Debug 技巧 / Pattern Generator

### 1. Python + Pattern Generator

建立你自己的 Pattern Generator 是一件超級有幫助的事，以下是一個簡單架構範例：

```python
class PatternGen:
    def __init__(self, filename):
        self.f = open(filename, 'w')

    def write_case(self, inputs):
        # e.g., inputs = {'in_valid': 1, 'op': 2, 'data': 14}
        line = f"{inputs['in_valid']}_{inputs['op']}_{inputs['data']}\n"
        self.f.write(line)

    def close(self):
        self.f.close()

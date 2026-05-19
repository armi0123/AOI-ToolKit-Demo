# AOI Vision Platform

## 中文介紹

這是一個使用 C# 與 Visual Studio 開發中的模組化 AOI 視覺檢測平台。

本專案的目標是建立一套可依照不同檢測需求，自由新增與選擇視覺檢測工具的 AOI 軟體架構，讓使用者能夠更直覺地建立檢測流程，同時保持介面乾淨、易於操作與維護。

目前開發方向包含：

* ROI 編輯工具
* Sobel 邊緣檢測
* 二值化參數調整
* 角點量測
* Tool 模組化架構
* 缺陷檢測研究

未來希望逐步新增：

* Blob 分析
* OCR / QRCode 辨識
* AI 瑕疵檢測
* 刮傷與髒污辨識
* Tool Flow 系統
* Recipe 管理功能

本專案也作為個人學習工業視覺、影像處理、AOI 系統設計與軟體架構開發的練習平台。

----------

## English Introduction

This is a modular AOI vision inspection platform currently under development using C# and Visual Studio.

The goal of this project is to create an expandable AOI software architecture that allows users to freely add and select vision inspection tools based on different inspection requirements.

I also hope to keep the user interface clean, intuitive, and easy to use, instead of having too many complicated tools displayed at once.

Current development features include:

* ROI Editor
* Sobel Edge Detection
* Threshold Adjustment
* Corner Measurement
* Modular Tool Architecture
* Defect Detection Research

Future development plans include:

* Blob Analysis
* OCR / QRCode Detection
* AI Defect Detection
* Scratch & Contamination Inspection
* Tool Flow System
* Recipe Management

This project is also used as a personal learning platform for industrial vision systems, image processing, AOI software design, and software architecture development.

----------
## 系統架構 (System Architecture)

AOI Vision Platform
│
├── Forms
│   ├── MainForm
│   ├── ROISettingForm
│   └── ToolSettingForm
│
├── Core
│   ├── Pipeline
│   ├── ToolResult
│   └── ImageManager
│
├── VisionTools
│   ├── ITool
│   ├── ToolBase
│   │
│   ├── ThresholdTool
│   ├── SobelTool
│   ├── CornerDetectTool
│   ├── QRCodeTool
│   ├── BarCodeTool
│   └── DataMatrixTool
│
├── ROI
│   ├── ROIObject
│   ├── ROIEditor
│   └── ROIManager
│
├── ImageProcessing
│   ├── EdgeDetection
│   ├── BinaryProcessing
│   └── FeatureDetection
│
├── Display
│   ├── ImageViewer
│   ├── OverlayRenderer
│   └── ResultDisplay
│
└── External Libraries
    ├── OpenCvSharp
    └── ZXing

----------
## 使用者介面 ( User Interface)

1.主畫面

<img width="762" height="385" alt="image" src="https://github.com/user-attachments/assets/ba82d784-a6fb-440c-93cd-2d0570d122e9" />

2.工具選擇畫面

<img width="620" height="383" alt="image" src="https://github.com/user-attachments/assets/3eaeea17-5fe7-45b7-b10e-0be07d22984e" />

3.工具參數設定畫面

<img width="619" height="382" alt="image" src="https://github.com/user-attachments/assets/45c96189-c001-4d8c-869b-9f28b11713ec" />

4.執行結果+結果輸出

<img width="761" height="385" alt="image" src="https://github.com/user-attachments/assets/ff49904d-b3d6-4c50-82a1-b8e5fbc185e8" />

----------

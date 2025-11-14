# 🚔 Police Image Converter (警務專用圖片處理助手)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Version](https://img.shields.io/badge/Version-v2.0-green)
![Features](https://img.shields.io/badge/Feature-Auto%20Resize-blue)

這是一個專為警務行政工作設計的**離線版**圖片處理工具。
它不僅能轉換 **HEIC/PNG** 格式，還能自動將圖片**縮放至符合 Word 表格的最佳尺寸**，大幅簡化後續製作筆錄的工作。

---

## ✨ v2.0 重大更新
* **📏 自動縮放 (Auto Resize)**：內建 **220 DPI** 高畫質演算法，將圖片像素調整至列印最佳大小。
* **🔀 雙模式分流**：
    * **一般照片**：自動縮放至 **13.5 x 8 cm** 範圍。
    * **手機截圖**：自動縮放至 **8 x 17 cm** 範圍。
* **⚡ 強制標準化**：即使原檔是 JPG，也會重新運算以確保尺寸符合規定，避免 Word 表格跑版。

## 🌟 核心特色
* **🔒 絕對資安**：全本機 (Client-side) 運算，照片**絕不**上傳伺服器。
* **📱 廣泛支援**：解決 iPhone HEIC 無法讀取問題，並修正 PNG 透明背景。
* **📦 一鍵打包**：處理完成後，自動分類並打包成 ZIP 下載。

## 🛠️ 使用教學
1. 開啟網頁，將所有照片拖曳至框框中。
2. 依據照片類型，點擊對應按鈕：
    * 若是刑案現場、監視器畫面 -> 點選 **「一般照片」**。
    * 若是 LINE 對話、網頁截圖 -> 點選 **「手機截圖」**。
3. 下載 ZIP 檔並解壓縮。
4. **直接匯入 Excel**：此時照片尺寸已完美，Excel 不需要再做額外運算，直接匯入即可。

## 🔧 技術規格
* **一般照片目標**：約 1169 x 693 px (等比縮放)
* **手機截圖目標**：約 693 x 1472 px (等比縮放)
* **輸出格式**：標準 JPEG (品質 92%, 白底)

---
## 📄 License
[MIT License](LICENSE)
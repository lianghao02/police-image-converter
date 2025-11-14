# 🚔 Police Image Converter (警務專用圖片轉檔助手)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Platform](https://img.shields.io/badge/Platform-Web%20(Client--Side)-blue)
![Security](https://img.shields.io/badge/Security-100%25%20Offline-brightgreen)

這是一個專為警務行政工作設計的**離線版**圖片轉檔工具。
旨在解決製作筆錄、移送書或刑案卷宗時，Excel/Word VBA 無法讀取 iPhone (HEIC) 或特殊格式圖片的問題。

**[🇬🇧 English Version](#english-description)**

---

## 🌟 核心特色 (Key Features)

* **🔒 絕對資安 (100% Secure)**：所有轉檔運算皆在**瀏覽器本機 (Client-side)** 執行，照片**絕不會**上傳至任何伺服器，確保案件資料無外洩風險。
* **⚡ 智慧優化**：自動偵測檔案格式。若原檔已是 JPG，則直接打包不重新壓縮，保留原始畫質並大幅提升速度。
* **📱 支援廣泛**：專門解決 iPhone 的 **HEIC** 格式，同時支援 PNG、WebP、BMP、AVIF、GIF。
* **⬜ 自動去背**：針對透明背景的圖片 (如 PNG/LINE 貼圖)，自動填充**白色背景**，避免放入 Word 時變黑底。
* **📦 一鍵打包**：轉檔完成後，自動將所有圖片打包成 ZIP 檔下載，檔名附帶時間戳記，方便歸檔。
* **🚀 無需安裝**：單一 HTML 檔案，無需安裝任何軟體，點擊即用。

## 🛠️ 使用方法 (How to Use)

### 方法一：線上直接使用 (GitHub Pages)
> *(如果您已開啟 GitHub Pages 功能，請在此處貼上您的網址，例如：)*
> [點擊這裡開啟工具](https://您的帳號.github.io/專案名稱/)

### 方法二：離線使用 (推薦公務電腦使用)
1.  點擊上方綠色的 **Code** 按鈕，選擇 **Download ZIP**。
2.  解壓縮下載的檔案。
3.  直接點兩下 `index.html` (或 `converter.html`)，使用 Chrome 或 Edge 瀏覽器開啟。
4.  將照片拖曳至網頁框框中，點擊「開始轉換」。

## 📂 支援格式列表

| 原始格式 | 轉換結果 | 說明 |
| :--- | :--- | :--- |
| **.HEIC / .HEIF** | .JPG | iPhone/iPad 拍攝的預設格式 (自動解碼) |
| **.PNG** | .JPG | 自動將透明背景轉為白色 |
| **.WEBP** | .JPG | 常見於網路下載或通訊軟體貼圖 |
| **.BMP** | .JPG | Windows 截圖或小畫家存檔 |
| **.AVIF** | .JPG | 新一代高壓縮格式 |
| **.JPG / .JPEG** | .JPG | **智慧略過** (不重新壓縮，直接打包) |

## ✨ v1.1 版本更新 (New in v1.1)
* **🔁 防重名機制**：自動偵測並重新命名重複的檔案 (例：`photo.jpg` -> `photo(1).jpg`)，避免批次處理時照片被覆蓋。
* **🔄 重置按鈕**：新增「清空重置」功能，方便進行多批次的連續轉檔作業。
* **⚡ 核心優化**：提升 JPG 智慧略過的判斷準確度。
## 🔧 技術架構 (Tech Stack)

本專案使用純 HTML5/JavaScript 開發，並引用以下開源函式庫 (透過 CDN)：

* [heic2any](https://github.com/alexcorvi/heic2any): 用於解碼 HEIC 檔案。
* [JSZip](https://stuk.github.io/jszip/): 用於在瀏覽器端建立 ZIP 壓縮檔。
* [FileSaver.js](https://github.com/eligrey/FileSaver.js/): 用於觸發檔案下載。

---

<a name="english-description"></a>
## 🇬🇧 English Description

### Police Image Converter (Offline Tool)

A secure, client-side tool designed to standardize evidence images for police paperwork automation. It converts various formats (HEIC, PNG, WebP) into standard **JPG** format, ensuring compatibility with Excel/Word VBA automation tools.

### Highlights
* **Privacy First**: Runs entirely in your browser. No files are uploaded to the server.
* **Smart Processing**: Skips re-compression for existing JPGs to preserve quality and speed.
* **HEIC Support**: Native conversion for iPhone photos.
* **Batch Processing**: Converts multiple files and downloads them as a single ZIP archive.

---

## 📄 License

本專案採用 [MIT License](LICENSE) 授權，歡迎自由使用、修改與分發。
# 中文詞彙分析工具 | Chinese Vocabulary Analyzer

一個專為華語文教學設計的詞彙分析工具，整合 TBCL（台灣華語文能力基準）斷詞系統，自動生成包含拼音和釋義的生詞表。

A vocabulary analysis tool designed for teaching Chinese as a second language, integrating TBCL (Taiwan Benchmarks for the Chinese Language) word segmentation system with automatic pinyin and definition generation.

## 🌟 功能特色 | Features

### 核心功能 | Core Features
- 📝 **文本輸入與分析** - 輸入中文文本並整合 TBCL 斷詞系統
- 📊 **CSV 檔案處理** - 上傳並解析 TBCL 斷詞結果
- 📚 **詞彙資料庫管理** - 建立已知詞彙資料庫，篩選生詞
- 🔍 **自動拼音查詢** - 自動查詢詞彙拼音（連寫格式）
- 📖 **自動釋義生成** - 自動提取簡潔的中文釋義
- 🏷️ **TBCL 等級標註** - 顯示詞彙的 TBCL 能力等級

### 進階功能 | Advanced Features
- ✂️ **手動切詞** - 可手動切分詞彙
- 🔗 **詞彙合併** - 可合併相鄰詞彙
- ✏️ **即時編輯** - 點擊欄位即可編輯拼音和釋義
- 📋 **生詞表顯示** - 美觀的表格式生詞列表
- 💾 **CSV 匯出** - 匯出包含完整資訊的 CSV 檔案
- 🖨️ **列印功能** - 直接列印或儲存為 PDF
- 📄 **文字複製** - 複製格式化的純文字生詞表

## 🚀 快速開始 | Quick Start

### 線上使用 | Online Use
1. 下載 `chinese-vocab-analyzer.html` 檔案
2. 使用瀏覽器開啟檔案（建議使用 Chrome、Firefox、Edge）
3. 開始使用！

### 本地部署 | Local Deployment
```bash
# 克隆專案
git clone https://github.com/your-username/chinese-vocab-analyzer.git

# 進入目錄
cd chinese-vocab-analyzer

# 使用瀏覽器開啟 HTML 檔案
open chinese-vocab-analyzer.html
```

## 📖 使用說明 | User Guide

### 完整工作流程 | Complete Workflow

#### 步驟 1：輸入文本 | Step 1: Input Text
1. 在「輸入文本」區域貼上或輸入需要分析的中文文本
2. 點擊「📋 複製文本」按鈕複製文本
3. 點擊「🔗 打開 TBCL 網站」前往 TBCL 斷詞系統

#### 步驟 2：TBCL 斷詞分析 | Step 2: TBCL Segmentation
1. 在 TBCL 網站（https://coct.naer.edu.tw/edit.jsp）貼上文本
2. 進行斷詞分析
3. 下載分析結果的 CSV 檔案

#### 步驟 3：上傳 CSV | Step 3: Upload CSV
1. 點擊「📁 選擇 CSV 檔案」上傳 TBCL 的斷詞結果
2. 系統會自動解析詞彙和等級資訊
3. 查看預覽確認上傳成功

#### 步驟 4：建立詞彙資料庫 | Step 4: Build Vocabulary Database
有兩種方式建立已知詞彙資料庫：

**方式 A：手動輸入**
- 在輸入框中輸入已知詞彙
- 按 Enter 或點擊「➕ 添加」按鈕

**方式 B：批次上傳**
- 準備包含已知詞彙的 .txt 或 .csv 檔案
- 點擊「📁 上傳詞彙檔案」上傳

#### 步驟 5：篩選生詞 | Step 5: Filter New Words
1. 點擊「🔍 對比並篩選生詞」按鈕
2. 系統自動對比並顯示未列入資料庫的生詞
3. 每個生詞顯示：
   - 詞彙本身
   - TBCL 等級（或「TBCL未收」）
   - 切詞/合併按鈕

#### 步驟 6：編輯詞彙（可選）| Step 6: Edit Words (Optional)
- **切詞**：點擊「切詞」按鈕，輸入切分位置
- **合併**：點擊「合併」按鈕，合併相鄰詞彙

#### 步驟 7：選擇生詞 | Step 7: Select Words
- 點擊生詞卡片選擇（選中後背景變紅色）
- 可選擇多個生詞

#### 步驟 8：生成生詞表 | Step 8: Generate Vocabulary List
1. 點擊「📋 顯示生詞表」按鈕
2. 系統自動查詢每個詞的拼音和釋義
3. 顯示查詢進度（例如：正在查詢... 5/10 (50%)）
4. 生成包含以下欄位的表格：
   - 編號
   - 詞彙
   - 拼音（連寫格式，如：zidong）
   - 釋義（簡潔的中文解釋）
   - TBCL 等級

#### 步驟 9：編輯與匯出 | Step 9: Edit & Export
**編輯拼音或釋義：**
- 點擊拼音或釋義欄位
- 直接輸入修改
- 點擊其他地方自動儲存

**匯出或複製：**
- 🖨️ **列印**：開啟列印對話框，可列印或儲存為 PDF
- 📋 **複製**：複製格式化的純文字到剪貼板
- 💾 **匯出 CSV**：下載包含所有資訊的 CSV 檔案

## 📄 授權 | License

MIT License

Copyright (c) 2026 Chinese Vocabulary Analyzer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.




## 🙏 致謝 | Acknowledgments

- **TBCL（台灣華語文能力基準）** - 提供詞彙等級標準
- **CC-CEDICT** - 中文字典資料
- **MDBG Chinese Dictionary** - 拼音和釋義查詢

## 📊 更新日誌 | Changelog

### v1.0.0 (2026-01-03)
- ✨ 初始版本發布
- 🎯 整合 TBCL 斷詞系統
- 🔍 自動拼音和釋義查詢
- 📊 生詞表生成與匯出
- 🎨 美觀的中國風介面設計



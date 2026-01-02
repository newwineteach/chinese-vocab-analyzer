# GitHub 上傳指南 | GitHub Upload Guide

## 📦 準備好的檔案 | Prepared Files

您的專案已經準備好以下檔案：

1. **chinese-vocab-analyzer.html** - 主要應用程式檔案
2. **index.html** - GitHub Pages 首頁（與主檔案相同）
3. **README.md** - 完整的專案說明文件
4. **LICENSE** - MIT 授權文件
5. **CONTRIBUTING.md** - 貢獻者指南
6. **.gitignore** - Git 忽略檔案設定
7. **.github/workflows/deploy.yml** - GitHub Pages 自動部署設定

## 🚀 上傳到 GitHub 的步驟 | Steps to Upload to GitHub

### 方式一：使用 GitHub 網頁介面 | Method 1: Using GitHub Web Interface

#### 步驟 1：建立新的儲存庫 | Step 1: Create a New Repository
1. 前往 [GitHub](https://github.com)
2. 點擊右上角的 ➕ → **New repository**
3. 填寫資訊：
   - **Repository name**: `chinese-vocab-analyzer`
   - **Description**: `中文詞彙分析工具 - 整合 TBCL 斷詞系統的華語文教學工具`
   - **Public** 或 **Private**（建議選 Public）
   - ❌ 不要勾選 "Add a README file"（我們已經有了）
   - ❌ 不要選擇 .gitignore 模板（我們已經有了）
   - ✅ 選擇 **License: MIT**（或跳過，我們已經有了）
4. 點擊 **Create repository**

#### 步驟 2：上傳檔案 | Step 2: Upload Files
1. 在新建立的儲存庫頁面，點擊 **uploading an existing file**
2. 將所有檔案拖曳到上傳區域：
   - chinese-vocab-analyzer.html
   - index.html
   - README.md
   - LICENSE
   - CONTRIBUTING.md
   - .gitignore
3. 在 "Commit changes" 區域：
   - Commit message: `Initial commit: Chinese Vocabulary Analyzer v1.0.0`
4. 點擊 **Commit changes**

#### 步驟 3：上傳 GitHub Actions 工作流程 | Step 3: Upload GitHub Actions Workflow
1. 在儲存庫中，點擊 **Add file** → **Create new file**
2. 檔案名稱輸入：`.github/workflows/deploy.yml`
3. 複製 `.github/workflows/deploy.yml` 的內容貼上
4. 點擊 **Commit changes**

### 方式二：使用 Git 命令列 | Method 2: Using Git Command Line

```bash
# 1. 在本地建立新目錄
mkdir chinese-vocab-analyzer
cd chinese-vocab-analyzer

# 2. 初始化 Git
git init

# 3. 複製所有檔案到這個目錄
# （從下載的輸出檔案中複製）

# 4. 添加檔案到 Git
git add .

# 5. 提交
git commit -m "Initial commit: Chinese Vocabulary Analyzer v1.0.0"

# 6. 連接到 GitHub 儲存庫（替換成您的 GitHub 用戶名）
git remote add origin https://github.com/YOUR-USERNAME/chinese-vocab-analyzer.git

# 7. 推送到 GitHub
git branch -M main
git push -u origin main
```

## 🌐 啟用 GitHub Pages | Enable GitHub Pages

### 步驟 1：前往設定 | Step 1: Go to Settings
1. 在您的儲存庫頁面，點擊 **Settings**
2. 在左側選單找到 **Pages**

### 步驟 2：設定來源 | Step 2: Configure Source
1. **Source** 選擇：`GitHub Actions`
2. 儲存設定

### 步驟 3：等待部署 | Step 3: Wait for Deployment
1. 前往 **Actions** 標籤
2. 查看部署進度
3. 部署完成後，會顯示網站網址

### 步驟 4：訪問網站 | Step 4: Visit Your Site
您的網站將會在：
```
https://YOUR-USERNAME.github.io/chinese-vocab-analyzer/
```

## ✅ 確認清單 | Verification Checklist

上傳完成後，請確認：

### GitHub 儲存庫 | GitHub Repository
- [ ] 所有檔案都已上傳
- [ ] README.md 正確顯示
- [ ] LICENSE 檔案存在
- [ ] .gitignore 檔案存在

### GitHub Pages
- [ ] Pages 已啟用
- [ ] 網站可以正常訪問
- [ ] 所有功能正常運作
- [ ] 樣式正確顯示

### 功能測試 | Function Testing
在 GitHub Pages 上測試：
- [ ] 輸入文本功能
- [ ] 複製功能
- [ ] 上傳 CSV
- [ ] 詞彙資料庫
- [ ] 生詞篩選
- [ ] 顯示生詞表
- [ ] 自動拼音查詢
- [ ] 匯出 CSV
- [ ] 列印功能
- [ ] 複製生詞表

## 📝 更新 README | Update README

記得更新 README.md 中的以下資訊：

1. **GitHub 儲存庫連結**：
```markdown
- GitHub Issues: [提交問題](https://github.com/YOUR-USERNAME/chinese-vocab-analyzer/issues)
```

2. **聯絡方式**：
```markdown
- Email: your-email@example.com
```

3. **線上 Demo 連結**：
在 README 開頭添加：
```markdown
## 🌐 線上使用 | Online Demo
👉 [立即使用 / Try Now](https://YOUR-USERNAME.github.io/chinese-vocab-analyzer/)
```

## 🎯 推廣您的專案 | Promote Your Project

### 添加主題標籤 | Add Topics
在儲存庫頁面右側，點擊設定圖示添加標籤：
- `chinese-language`
- `chinese-learning`
- `education`
- `vocabulary`
- `teaching-tool`
- `tbcl`
- `language-learning`
- `pinyin`

### 建立發布版本 | Create a Release
1. 前往 **Releases**
2. 點擊 **Create a new release**
3. Tag: `v1.0.0`
4. Release title: `v1.0.0 - Initial Release`
5. 描述主要功能
6. 點擊 **Publish release**

### 分享到社群 | Share to Community
- 分享到 Reddit: r/ChineseLanguage
- 分享到 Twitter/X
- 分享到相關的教育論壇
- 通知華語文教學社群

## 🔧 常見問題 | Troubleshooting

### Q: GitHub Pages 顯示 404
A: 確認：
- Pages 已啟用
- 分支設定正確
- index.html 檔案存在
- 等待幾分鐘讓 GitHub 部署

### Q: 檔案上傳失敗
A: 
- 檢查檔案大小（單檔不超過 100MB）
- 確認網路連線
- 嘗試分批上傳

### Q: 功能在 GitHub Pages 上不工作
A: 
- 檢查瀏覽器控制台的錯誤訊息
- 確認 API 呼叫沒有 CORS 問題
- 檢查是否為 HTTPS 問題

## 📞 需要協助？ | Need Help?

如果遇到問題：
1. 查看 [GitHub 文件](https://docs.github.com/)
2. 搜尋相關的錯誤訊息
3. 在 GitHub Discussions 發問
4. 聯絡 GitHub 支援

## 🎉 完成！ | Done!

恭喜！您的中文詞彙分析工具現在已經在 GitHub 上了，全世界的華語文教師和學習者都可以使用它！

Congratulations! Your Chinese Vocabulary Analyzer is now on GitHub and available to Chinese language teachers and learners worldwide!

---

**祝您的專案成功！Good luck with your project! 🚀**

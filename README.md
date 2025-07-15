# 📝 Prompt 模板填入工具

一個專為 AI prompt 設計的模板管理和填入工具，讓您輕鬆建立、管理和使用可重複的 prompt 模板。

🔗 **線上使用：** [https://fill.prompt.owo.is](https://fill.prompt.owo.is)

## ✨ 主要功能

### 🎯 核心功能
- **模板編輯器**：支援使用 `[變數]` 語法建立 prompt 模板
- **互動式填入**：點擊模板中的占位符即可填入具體內容
- **格式分類系統**：提供五大類格式要求快速按鈕
- **智慧衝突檢測**：自動移除互斥的格式要求
- **URL 分享**：透過 URL 參數分享模板給他人
- **一鍵複製**：將完整的 prompt 複製到剪貼簿

### 🎨 格式分類
1. **📊 輸出格式**：表格、清單、JSON、段落
2. **📏 長度控制**：50字、100字、詳細分析、摘要
3. **🏗️ 結構要求**：分點、步驟、問答、比較
4. **🎯 語言風格**：專業、淺顯、商業、學術
5. **📋 特殊要求**：例子、數據、可行性、建議

## 🚀 快速開始

### 線上使用
直接訪問 [線上版本](https://fill.prompt.owo.is) 即可開始使用。

### 本地使用
```bash
# 下載專案
git clone https://github.com/yourusername/prompt-template.git
cd prompt-template

# 啟動本地伺服器（任選其一）
python -m http.server 8000
# 或
npx serve .

# 開啟瀏覽器訪問
open http://localhost:8000
```

## 📖 使用說明

### 1. 建立模板
點擊「編輯模板」按鈕，使用 `[變數名稱]` 語法建立模板：

```
請幫我找出 [產品類型/族群] 在 [市場區域] 的使用行為與購買趨勢，並說明主要的消費動機與痛點。
```

### 2. 填入變數
點擊模板中的藍色標籤，在彈出視窗中填入具體內容。

### 3. 添加格式要求
使用下方的分類按鈕快速添加格式要求，系統會自動處理衝突的格式。

### 4. 複製使用
點擊「複製結果」按鈕，將完整的 prompt 複製到剪貼簿。

## 🔗 分享模板

### URL 分享
在模板編輯器中點擊「複製分享連結」，可以產生包含模板的 URL：
```
https://fill.prompt.owo.is/?prompt=你的模板內容
```

## 🛠 技術特色

- **零依賴**：純 vanilla JavaScript，無需任何外部函式庫
- **單檔案應用**：所有功能包含在一個 HTML 檔案中
- **即開即用**：無需建置過程，直接開啟即可使用
- **響應式設計**：適配桌面和行動裝置
- **現代化介面**：美觀的漸層設計和流暢動畫

## 🎯 適用場景

### 使用者群體
- AI 工具使用者
- 內容創作者
- 市場分析師
- 產品經理
- 研究人員

### 應用場景
- 市場調研 prompt 模板
- 內容創作 prompt 模板
- 資料分析 prompt 模板
- 產品分析 prompt 模板
- 學術研究 prompt 模板

## ⌨️ 快捷鍵

- `ESC`：關閉彈出視窗
- `Enter`：確認填入內容
- `Ctrl+C`：複製最終結果
- `Ctrl+Enter`：在模板編輯器中儲存模板

## 🌐 瀏覽器支援

- Chrome 67+
- Firefox 79+
- Safari 14.1+
- Edge 79+

## 📁 專案結構

```
prompt-template/
├── index.html          # 主要應用程式檔案
├── package.json        # 專案配置
├── README.md           # 說明文件
├── CHANGELOG.md        # 版本更新記錄
├── changelogs/         # 詳細版本記錄
│   ├── unreleased.md   # 未發佈功能
│   └── v1.0.0.md      # v1.0.0 版本記錄
└── .github/
    └── workflows/      # GitHub Actions 設定
        ├── deploy.yml  # GitHub Pages 部署
        └── release.yml # 自動發佈流程
```

## 🤝 貢獻

歡迎提交 Issue 和 Pull Request！

## 📄 授權

MIT License

---

⭐ 如果這個工具對您有幫助，請給個星星支持！
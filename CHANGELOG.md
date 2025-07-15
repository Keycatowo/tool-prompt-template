# 更新日誌

這是 Prompt 模板填入工具的主要更新日誌概覽。

📁 **詳細的版本記錄請查看 `changelogs/` 資料夾中的各版本文件。**

## 版本列表

- [**未發佈**](changelogs/unreleased.md) - 計劃中的功能和改進
- [**v0.1.0-alpha**](changelogs/v0.1.0-alpha.md) - 2025-07-15 - Alpha 版本發布

## 版本記錄說明

每個版本的詳細變更記錄都存放在 `changelogs/` 資料夾中：

- `unreleased.md` - 記錄未發佈的功能和計劃
- `vX.X.X.md` - 記錄對應版本的完整變更內容

## 自動化發佈

本專案使用 GitHub Actions 自動化發佈流程：

1. 在 `dev` 分支建立 `vX.X.X` 格式的標籤
2. 自動合併到 `main` 分支
3. 自動建立 GitHub Release
4. Release 內容來自對應版本的 changelog 文件
5. 自動部署到 GitHub Pages

---

日誌格式基於 [Keep a Changelog](https://keepachangelog.com/zh-TW/1.0.0/)，
並遵循 [語義化版本控制](https://semver.org/lang/zh-TW/)。
# Shellback SVN

![TortoiseSVN-Style](https://img.shields.io/badge/TortoiseSVN%20❤️-red)
![平台](https://img.shields.io/badge/平台-Windows%20%7C%20macOS%20%7C%20Linux-success)
[![VS Code 市集](https://img.shields.io/visual-studio-marketplace/v/Shellback.shellback-svn?label=VS%20Code%20市集&color=007ACC)](https://marketplace.visualstudio.com/items?itemName=Shellback.shellback-svn)
[![OpenVSX](https://img.shields.io/open-vsx/v/Shellback/shellback-svn?label=OpenVSX&color=007ACC)](https://open-vsx.org/extension/Shellback/shellback-svn)
[![GitHub Issues](https://img.shields.io/github/issues/shellback-labs/shellback-svn)](https://github.com/shellback-labs/shellback-svn/issues)

[English](./README.md) | [简体中文](./README.zh-CN.md) | [繁體中文](./README.zh-TW.md) | [日本語](./README.ja.md) | [한국어](./README.ko.md)

**熟悉的右鍵選單工作流程，專為 VS Code 打造。**

懷念 TortoiseSVN 的右鍵效率？Shellback SVN 將經典的檔案樹驅動 SVN 工作流程帶到 VS Code——無需命令面板，無需學習曲線，工具就在您期望的位置。

## 🚀 功能特色

#### TortoiseSVN 風格

熟悉的視覺化回饋，與桌面 SVN 客戶端一致

#### SVN 更新
![SVN 更新示範](resources/rightclick-update.gif)

更新檔案或整個工作副本

#### SVN 提交
![SVN 提交示範](resources/rightclick-commit.gif)

提交對話方塊，包含訊息歷程記錄和自動偵測新增/刪除檔案

#### SVN 還原
![SVN 還原示範](resources/rightclick-revert.gif)

還原單一或多個檔案，帶確認對話方塊

- **顯示記錄**：三欄記錄檢視器，顯示提交歷程、訊息和變更的檔案
- **衝突解決**：視覺化衝突面板，提供解決選項（使用我的/使用他們的/編輯/差異比對）

## 📋 系統需求

### VS Code
- **版本**：1.80.0 或更高

### SVN 命令列客戶端
Shellback SVN 需要在您的系統上安裝 SVN CLI。

**安裝方式：**
- **macOS**：透過 [Homebrew](https://brew.sh/) 安裝（`brew install subversion`）
- **Windows**：[TortoiseSVN](https://tortoisesvn.net/downloads.html)（安裝時勾選「命令列客戶端工具」）
- **Linux**：使用您的發行版套件管理員或造訪 [Apache SVN 官方下載頁面](https://subversion.apache.org/packages.html)

安裝後，重新啟動 VS Code 以確保其識別 SVN 命令。

## 🎯 快速開始

1. **安裝** 從 VS Code 市集安裝 Shellback SVN
2. **開啟** 包含 SVN 工作副本的資料夾
3. **按右鍵** 檔案總管檢視中的任何檔案或資料夾
4. **選擇** 右鍵選單中的 SVN 命令

**提示**：按住 `Alt` 鍵（macOS：`Option`）同時點擊選單項目，可對目前工作區根目錄（您開啟的資料夾）執行操作。

## 🤝 回饋與支援

發現 Bug 或有功能建議？請在 [GitHub](https://github.com/shellback-labs/shellback-svn/issues) 上提交問題。

---

**注意**：此擴充功能旨在成為 SVN CLI 和 VS Code UI 之間的輕量級橋樑。它專注於恢復多年來許多開發者所依賴的「右鍵點擊」生產力。無遙測，無臃腫。

# Shellback SVN

![TortoiseSVN-Style](https://img.shields.io/badge/TortoiseSVN%20❤️-red)
![平台](https://img.shields.io/badge/平台-Windows%20%7C%20macOS%20%7C%20Linux-success)
[![VS Code 市场](https://img.shields.io/visual-studio-marketplace/v/Shellback.shellback-svn?label=VS%20Code%20市场&color=007ACC)](https://marketplace.visualstudio.com/items?itemName=Shellback.shellback-svn)
[![OpenVSX](https://img.shields.io/open-vsx/v/Shellback/shellback-svn?label=OpenVSX&color=007ACC)](https://open-vsx.org/extension/Shellback/shellback-svn)
[![GitHub Issues](https://img.shields.io/github/issues/shellback-labs/shellback-svn)](https://github.com/shellback-labs/shellback-svn/issues)

[English](./README.md) | [简体中文](./README.zh-CN.md) | [繁體中文](./README.zh-TW.md) | [日本語](./README.ja.md) | [한국어](./README.ko.md)

**熟悉的右键菜单工作流，专为 VS Code 打造。**

通过 Tortoise 风格的上下文菜单，直接从 VS Code 文件资源管理器执行 SVN 命令。

注意：此扩展需要安装 SVN CLI 并将其添加到系统 PATH 中。

## 🚀 功能特性

#### TortoiseSVN 风格

熟悉的可视化反馈，与桌面 SVN 客户端一致

#### SVN 更新
![SVN 更新演示](resources/rightclick-update.gif)

更新文件或整个工作副本

#### SVN 提交
![SVN 提交演示](resources/rightclick-commit.gif)

提交对话框，包含消息历史记录和自动检测新增/删除文件

#### SVN 还原
![SVN 还原演示](resources/rightclick-revert.gif)

还原单个或多个文件，带确认对话框

#### 显示日志
![显示日志截图](resources/rightclick-showlog.png)

三栏日志查看器，显示提交历史、消息和更改的文件

#### 冲突解决
![冲突截图](resources/resolve-conflicts.png)

可视化冲突面板，提供解决选项（使用我的/使用他们的/编辑/差异对比）

## 📋 系统要求

### VS Code
- **版本**：1.80.0 或更高

### SVN 命令行客户端
Shellback SVN 需要在您的系统上安装 SVN CLI。

**安装方式：**
- **macOS**：通过 [Homebrew](https://brew.sh/) 安装（`brew install subversion`）
- **Windows**：[TortoiseSVN](https://tortoisesvn.net/downloads.html)（安装时勾选"命令行客户端工具"）
- **Linux**：使用您的发行版包管理器或访问 [Apache SVN 官方下载页面](https://subversion.apache.org/packages.html)

安装后，重启 VS Code 以确保其识别 SVN 命令。

## 🎯 快速开始

1. **安装** 从 VS Code 市场安装 Shellback SVN
2. **打开** 包含 SVN 工作副本的文件夹
3. **右键单击** 资源管理器视图中的任何文件或文件夹
4. **选择** 上下文菜单中的 SVN 命令

**提示**：按住 `Alt` 键（macOS：`Option`）同时点击菜单项，可对当前工作区根目录（您打开的文件夹）执行操作。

## 🤝 反馈与支持

发现 Bug 或有功能建议？请在 [GitHub](https://github.com/shellback-labs/shellback-svn/issues) 上提交问题。

---

**注意**：此扩展旨在成为 SVN CLI 和 VS Code UI 之间的轻量级桥梁。它专注于恢复多年来许多开发者所依赖的"右键单击"生产力。无遥测，无臃肿。

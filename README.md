# Shellback SVN

[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/Shellback.shellback-svn?label=VS%20Code%20Marketplace&color=007ACC)](https://marketplace.visualstudio.com/items?itemName=Shellback.shellback-svn)
[![OpenVSX](https://img.shields.io/open-vsx/v/Shellback/shellback-svn?label=OpenVSX&color=007ACC)](https://open-vsx.org/extension/Shellback/shellback-svn)
[![VS Code Version](https://img.shields.io/badge/VS%20Code-%3E%3D1.80.0-blue)](https://code.visualstudio.com/)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-success)](https://code.visualstudio.com/)
[![GitHub Issues](https://img.shields.io/github/issues/shellback-labs/shellback-svn)](https://github.com/shellback-labs/shellback-svn/issues)

**The familiar context-menu workflow, built for VS Code.**

Missing TortoiseSVN's right-click efficiency? Shellback SVN brings the classic file-tree-driven SVN workflow to VS Code—no command palette required, no learning curve, just the tools you need right where you expect them.

## 🚀 Features

#### TortoiseSVN-Style

Familiar visual feedback matching desktop SVN clients

#### SVN Update
![SVN Update Demo](resources/rightclick-update.gif)

Update files or entire working copy

#### SVN Commit
![SVN Commit Demo](resources/rightclick-commit.gif)

Commit dialog with message history and automatic detection of new/deleted files

#### SVN Revert
![SVN Revert Demo](resources/rightclick-revert.gif)

Revert single or multiple files with confirmation dialogs

- **Show Log**: Three-pane log viewer displaying commit history, messages, and changed files
- **Conflict Resolution**: Visual conflict panel with resolution options (Use Mine/Theirs/Edit/Diff)

## 📋 Requirements

### VS Code
- **Version**: 1.80.0 or higher

### SVN Command Line Client
Shellback SVN requires the SVN CLI to be installed on your system.


**Installation:**
- **macOS**: Install via [Homebrew](https://brew.sh/) (`brew install subversion`)
- **Windows**: [TortoiseSVN](https://tortoisesvn.net/downloads.html) (check "command line client tools" during installation)
- **Linux**: Use your distribution's package manager or see the [official Apache SVN download page](https://subversion.apache.org/packages.html)

After installation, restart VS Code to ensure it recognizes the SVN command.

## 🎯 Quick Start

1. **Install** Shellback SVN from the VS Code Marketplace
2. **Open** a folder containing an SVN working copy
3. **Right-click** any file or folder in the Explorer view
4. **Select** SVN commands from the context menu

**Tip**: Hold `Alt` (macOS: `Option`) while clicking menu items to perform operations on the current workspace root (the folder you have open).

## 🤝 Feedback & Support

Found a bug or have a feature request? Please open an issue on [GitHub](https://github.com/shellback-labs/shellback-svn/issues).

---

**Note**: This extension is designed to be a lightweight bridge between the SVN CLI and VS Code UI. It focuses on restoring the "Right-Click" productivity that many developers relied on for years. No telemetry, no bloat.

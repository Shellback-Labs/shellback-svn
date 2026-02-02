# Shellback SVN

**The familiar context-menu workflow, built for VS Code.**

Missing TortoiseSVN's right-click efficiency? Shellback SVN brings the classic file-tree-driven SVN workflow to VS Code—no command palette required, no learning curve, just the tools you need right where you expect them.

## ✨ What Makes Shellback Different

- **Context-First Design**: Right-click files/folders in Explorer to access all SVN commands
- **TortoiseSVN Parity**: Pre-commit update checks, visual log viewer, conflict resolution—all familiar workflows
- **Dual-Mode Commands**: Operations on selected items or entire working copy (Alt+Click for root operations)
- **Zero Configuration**: Uses your existing SVN CLI installation—no server setup, no authentication hassle
- **Lightweight & Fast**: Direct CLI integration with no bloat or telemetry

## 🚀 Key Features

### Icon Overlays/Status Badges
- **Status Indicators**: Files show their SVN status directly in Explorer (M/A/D/C/U/!)
- **Color Coding**: Modified files appear in blue, added in green, conflicts in orange
- **Folder Indicators**: Folders show a dot when containing modified files
- **TortoiseSVN-Style**: Familiar visual feedback matching desktop SVN clients

### Core Operations

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

### TortoiseSVN-Style Workflows
- **Pre-Commit Update Check**: Detects out-of-date working copy before committing, with one-click update option
- **Auto-Add/Delete**: Automatically detects and handles unversioned and missing files during commit
- **Commit Message History**: Dropdown menu for reusing recent commit messages

### Additional Commands
- **SVN Add**: Add unversioned files to version control
- **SVN Delete**: Mark files for deletion from repository
- **SVN Cleanup**: Fix interrupted operations and working copy locks

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

**Tip**: Hold `Alt` (macOS: `Option`) while clicking menu items to perform operations on the entire working copy root.

## 🤝 Feedback & Support

Found a bug or have a feature request? Please open an issue on [GitHub](https://github.com/shellback-labs/shellback-svn/issues).

---

**Note**: This extension is designed to be a lightweight bridge between the SVN CLI and VS Code UI. It focuses on restoring the "Right-Click" productivity that many developers relied on for years. No telemetry, no bloat.

# Shellback SVN

![TortoiseSVN-Style](https://img.shields.io/badge/TortoiseSVN%20❤️-red)
![プラットフォーム](https://img.shields.io/badge/プラットフォーム-Windows%20%7C%20macOS%20%7C%20Linux-success)
[![VS Code マーケットプレイス](https://img.shields.io/visual-studio-marketplace/v/Shellback.shellback-svn?label=VS%20Code%20マーケットプレイス&color=007ACC)](https://marketplace.visualstudio.com/items?itemName=Shellback.shellback-svn)
[![OpenVSX](https://img.shields.io/open-vsx/v/Shellback/shellback-svn?label=OpenVSX&color=007ACC)](https://open-vsx.org/extension/Shellback/shellback-svn)
[![GitHub Issues](https://img.shields.io/github/issues/shellback-labs/shellback-svn)](https://github.com/shellback-labs/shellback-svn/issues)

[English](./README.md) | [简体中文](./README.zh-CN.md) | [繁體中文](./README.zh-TW.md) | [日本語](./README.ja.md) | [한국어](./README.ko.md)

**VS Code のための、使い慣れたコンテキストメニューワークフロー。**

TortoiseSVN の右クリック効率が恋しいですか？Shellback SVN は、クラシックなファイルツリー駆動の SVN ワークフローを VS Code に提供します。コマンドパレット不要、学習曲線なし、必要なツールを期待する場所で利用できます。

## 🚀 機能

#### TortoiseSVN スタイル

デスクトップ SVN クライアントと同じ、使い慣れたビジュアルフィードバック

#### SVN 更新
![SVN 更新デモ](resources/rightclick-update.gif)

ファイルまたは作業コピー全体を更新

#### SVN コミット
![SVN コミットデモ](resources/rightclick-commit.gif)

メッセージ履歴と新規/削除ファイルの自動検出を備えたコミットダイアログ

#### SVN 復元
![SVN 復元デモ](resources/rightclick-revert.gif)

確認ダイアログ付きで単一または複数のファイルを復元

#### ログ表示
![ログ表示スクリーンショット](resources/rightclick-showlog.png)

コミット履歴、メッセージ、変更されたファイルを表示する3ペインログビューア

#### 競合解決
![競合スクリーンショット](resources/resolve-conflicts.png)

解決オプション（自分の変更を使用/相手の変更を使用/編集/差分）を備えたビジュアル競合パネル

## 📋 必要環境

### VS Code
- **バージョン**：1.80.0 以上

### SVN コマンドラインクライアント
Shellback SVN を使用するには、システムに SVN CLI がインストールされている必要があります。

**インストール方法：**
- **macOS**：[Homebrew](https://brew.sh/) 経由でインストール（`brew install subversion`）
- **Windows**：[TortoiseSVN](https://tortoisesvn.net/downloads.html)（インストール時に「コマンドラインクライアントツール」をチェック）
- **Linux**：ディストリビューションのパッケージマネージャーを使用するか、[Apache SVN 公式ダウンロードページ](https://subversion.apache.org/packages.html)を参照

インストール後、VS Code を再起動して SVN コマンドが認識されることを確認してください。

## 🎯 クイックスタート

1. **インストール** VS Code マーケットプレイスから Shellback SVN をインストール
2. **開く** SVN 作業コピーを含むフォルダーを開く
3. **右クリック** エクスプローラービューで任意のファイルまたはフォルダーを右クリック
4. **選択** コンテキストメニューから SVN コマンドを選択

**ヒント**：メニュー項目をクリックする際に `Alt`（macOS：`Option`）キーを押したままにすると、現在のワークスペースルート（開いているフォルダー）に対して操作を実行できます。

## 🤝 フィードバックとサポート

バグを見つけたり、機能リクエストがありますか？[GitHub](https://github.com/shellback-labs/shellback-svn/issues) で Issue を開いてください。

---

**注意**：この拡張機能は、SVN CLI と VS Code UI の間の軽量なブリッジとして設計されています。多くの開発者が長年頼りにしてきた「右クリック」の生産性を復元することに焦点を当てています。テレメトリなし、肥大化なし。

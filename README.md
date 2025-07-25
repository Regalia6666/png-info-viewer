<img width="1717" height="813" alt="Image" src="https://github.com/user-attachments/assets/23c0545d-2653-4ee2-843c-1da2f1cb40b3" />

# PNG Info Viewer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**PNG Info Viewer** は、ウェブページ上のPNG画像に埋め込まれた情報を手軽に確認できるChrome拡張機能です。右クリックするだけで、画像の解像度、ファイルサイズ、そして`tEXt`チャンクに格納されたメタデータを瞬時に表示します。

## ✨ 機能

*   **右クリックから即時表示**: 画像の上で右クリックし、メニューを選択するだけで情報を表示します。
*   **詳細な画像情報**: 以下の情報を分かりやすく表示します。
    *   **px数**: 画像の本来のピクセル解像度 (例: 1920 x 1080)
    *   **ファイルサイズ**: 読みやすい単位 (KB, MB) に変換されたサイズ
    *   **ファイル名**: URLから抽出したファイル名
    *   **PNGinfo**: PNGファイルの`tEXt`チャンクから抽出したメタデータ（キーワードとテキストのペア）
*   **見やすいダイアログ**: ページ前面にオーバーレイ表示されるため、ページ遷移することなく情報を確認できます。

## 🚀 インストール方法

1.  このリポジトリの最新リリースをダウンロードし、ZIPファイルを解凍します。
    *   または、`git clone https://github.com/あなたのユーザー名/png-info-viewer.git` でリポジトリをクローンします。
2.  Chromeブラウザを開き、アドレスバーに `chrome://extensions` と入力して拡張機能管理ページに移動します。
3.  ページの右上にある **「デベロッパーモード」** のスイッチをオンにします。
4.  **「パッケージ化されていない拡張機能を読み込む」** というボタンをクリックします。
5.  ファイル選択ダイアログで、手順1で解凍（またはクローン）した `png-info-viewer` フォルダを選択します。
6.  拡張機能の一覧に「PNG Info Viewer」が表示されれば、インストールは完了です。

## 使い方

1.  情報を確認したいPNG画像が表示されているウェブページを開きます。
2.  画像の上でマウスを右クリックします。
3.  コンテキストメニューから **「png-info-viewer で情報を表示」** をクリックします。
4.  ページの前面に情報の詳細が記載されたダイアログが表示されます。
5.  ダイアログの外側をクリックするか、`Esc`キーを押すとダイアログが閉じます。

## 🛠️ 技術スタック

*   **Manifest V3**: 最新のChrome拡張機能プラットフォーム
*   **JavaScript (ES6+)**: 機能の主要ロジック
*   **HTML / CSS**: 情報表示用のダイアログ
*   **Chrome APIs**:
    *   `chrome.contextMenus`: 右クリックメニューの作成
    *   `chrome.scripting`: ウェブページへのスクリプト注入
    *   `chrome.tabs`: タブ間でのメッセージング

## 🤝 コントリビュート

バグ報告、機能提案、プルリクエストなどを歓迎します！
Issueを立てるか、このリポジトリをフォークして変更を加え、プルリクエストを送信してください。

---

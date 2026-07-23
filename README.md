# ボウヤ制作アプリ

個人開発したWindows向け小型ツールをまとめて紹介する、GitHub Pages向けの静的サイトです。各アプリの紹介、GitHubリポジトリ、Releases、開発支援、作者情報への導線を掲載します。

## ローカルで確認する

`index.html` をWebブラウザで直接開いてください。ビルドや依存パッケージのインストールは不要です。

## ファイル構成

```text
BouyaAppsSite/
├─ index.html
├─ styles.css
├─ README.md
├─ .gitignore
└─ assets/
   ├─ pomodoro-overlay-icon.png
   ├─ bakusoku-screenshot-icon.png
   └─ site-icon.png
```

アイコン画像が未配置でも、各アプリカードにはCSSによるプレースホルダーが表示されます。画像を用意したら、上記のファイル名で `assets` フォルダに配置してください。

## GitHub Pagesで公開する

推奨リポジトリ名は `<GitHubユーザー名>.github.io` です。

1. このフォルダの内容をGitHubリポジトリのルートへ配置します。
2. GitHubのリポジトリ設定から **Pages** を開きます。
3. Sourceを **Deploy from a branch** にします。
4. Branchを **main**、Folderを **/(root)** にして保存します。
5. `https://<GitHubユーザー名>.github.io/` を開いて確認します。

## 差し替えが必要なURL

`index.html` 内の次のTODOリンクを、確定した実URLへ差し替えてください。

- `#TODO-POMODORO-GITHUB` — PomodoroOverlayのGitHubリポジトリ
- `#TODO-POMODORO-RELEASES` — PomodoroOverlayのGitHub Releases
- `#TODO-SCREENSHOT-GITHUB` — BakusokuScreenshotのGitHubリポジトリ
- `#TODO-SCREENSHOT-RELEASES` — BakusokuScreenshotのGitHub Releases
- `#TODO-AUTHOR-GITHUB` — 作者のGitHubプロフィール

OFUSE（`https://ofuse.me/df740631`）とX（`https://x.com/xbouyax`）は設定済みです。

## 更新時の基本手順

1. `index.html` の内容を更新します。
2. 必要に応じて `styles.css` と `assets` 内の画像を更新します。
3. PC幅とスマートフォン幅で表示とリンクを確認します。
4. 変更を `main` ブランチへ反映します。
5. GitHub Pagesの公開ページで最終確認します。

アプリを増やす場合は、`index.html` の `.app-card` を複製し、名称、説明、状態、アイコン、リンクを差し替えます。

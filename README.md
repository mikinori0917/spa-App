# SPA アプリ（GitHub Pages 用スターター）

このフォルダをそのまま GitHub にアップロードすれば、GitHub Pages で公開できます。

## 公開手順（ブラウザだけでOK）
1. GitHub にログイン → 右上の「＋」→ **New repository**。
2. Repository name を `spa-app`（任意）にして **Create repository**。
3. ファイル一覧の画面で **Add file → Upload files** を押し、本フォルダ内の **index.html** と **manifest.webmanifest** をドラッグ&ドロップ → **Commit changes**。
4. リポジトリの **Settings → Pages** を開き、
   - Source: **Deploy from a branch**
   - Branch: **main / root** を選択 → **Save**。
5. 数十秒後に `https://<GitHubユーザー名>.github.io/<リポジトリ名>/` で公開されます。

> ルート直下に **index.html** があることが重要です。

## 注意点
- 音声はブラウザの仕様により、ページを一度タップ/クリックしてから有効になります（画面左上の「音声: 無効（ページをクリック）」の表示が「有効」になればOK）。
- スマホでバイブ/音を動かすには、**HTTPS** + **ユーザー操作**（タップ）が必要です。GitHub Pages は HTTPS なので問題ありません。
- 位置情報（GPS）はブラウザからの許可が必要です。

## 追加の使い方
- 公開URLが `https://<user>.github.io/spa-app/` の場合、ブックマークやホーム画面追加（PWA）はそのURLを指定してください。
- 詳細な調整は `index.html` を直接編集してコミットすれば即反映されます。

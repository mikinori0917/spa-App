# SPA Monitor (GitHub Pages Package)

このフォルダの `index.html` をリポジトリのルートに置き、GitHub Pages を「main ブランチ / ルート」に設定すると公開できます。

## 手順（簡易）
1. GitHubで新規リポジトリを作成（例: `spa-monitor`）。**Public** を推奨。
2. `Add file` → `Upload files` で `index.html` と `manifest.webmanifest` をアップロードし、`Commit changes`。
3. `Settings` → `Pages` → **Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / **/(root)** を選択 → `Save`
4. 数十秒後、`https://<ユーザー名>.github.io/spa-monitor/` で公開されます。

※ このアプリは外部CDNに依存しない設計のため、単一HTMLとしてそのまま動作します。
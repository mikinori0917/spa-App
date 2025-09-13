
# SPA Monitor (GitHub Pages)

このリポジトリは、ブラウザだけで動作する**SPA（Spatial Probability Anomaly）モニター**の配布用です。  
`index.html` を GitHub Pages で公開すればインストール不要で動作します。

## 公開手順（GitHub Pages）
1. GitHubで新規リポジトリを作成（例: `spa-monitor`）。`Public` を選択。
2. このフォルダ内のファイルを**そのまま**リポジトリ直下にアップロード。  
   - `index.html`  
   - `manifest.webmanifest`  
   - `icons/` フォルダ（アイコン）  
   - `.nojekyll`
3. GitHub の **Settings → Pages** を開き、
   - **Source**: `Deploy from a branch`
   - **Branch**: `main`（または `master`）/ `/ (root)` を選択 → **Save**
4. 数十秒後、`https://<GitHubユーザー名>.github.io/<リポジトリ名>/` でアクセス可能。

## カスタムドメイン（任意）
- Settings → Pages → **Custom domain** にドメインを入力し、DNSに `CNAME` を設定。

## 変更点（本パッケージ）
- `SPAレベルBの集計期間`: デフォルト **3秒**
- `バイブ用しきい値`: Inst / A / B **2.0**

## ローカル動作
- ダブルクリックで `index.html` を開くだけで動作します（外部CDN不要）。


# SPA Monitor (PWA版) 簡易配布パッケージ

このフォルダを **HTTPS で公開** すると、Safari/Chrome から
「ホーム画面に追加」で “アプリ化” できます（オフライン動作対応）。

## 使い方（最短）
1. このZIPを解凍してフォルダごとホスティング（GitHub Pages / Cloudflare Pages / Netlify など）
2. 公開URLを配布（QRコード・LINE・メール等）
3. 受け取った人は Safari/Chrome でURLを開き → 共有 → ホーム画面に追加

※ iOS の Geolocation と WebAudio は https 上でのみ安定動作します（file://では制限あり）。

## ローカル確認（開発用）
- “Live Server” 等のローカルHTTPで index.html を表示すればOK。


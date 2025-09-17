# SPAリアルタイム異常検知アプリ（GitHub Pages 用パック）

このフォルダをそのまま GitHub リポジトリにアップロードすれば、**GitHub Pages** で公開できます。（`index.html` 単一ファイル＋アイコン＋ `manifest.webmanifest` の構成です）

## 公開手順（最短）
1. GitHubで新規リポジトリを作成（例: `spa-monitor`）。
2. このフォルダ内のファイル一式をそのリポジトリのルート（直下）にアップロード。  
   - もしくは `Add file > Upload files` からドラッグ＆ドロップ。
3. **Settings > Pages** を開き、
   - **Build and deployment**: `Deploy from a branch`
   - **Branch**: `main` / `/ (root)` を選択して **Save**。
4. 数十秒〜数分後、`https://<あなたのユーザー名>.github.io/<リポジトリ名>/` で公開されます。

## ファイル構成
- `index.html` : アプリ本体（オフライン完結、外部CDN不要）
- `manifest.webmanifest` : PWA用マニフェスト（本体HTMLの参照と整合）
- `icons/icon-192.png`, `icons/icon-512.png` : アイコン
- `LICENSE` : MITライセンス
- `README.md` : この説明

## よくある質問（FAQ）
- **CSVのファイル名が期待通りにならない**  
  ブラウザの挙動や権限・ダイアログ表示の差で見え方が変わる場合があります。ダウンロード名は `場所_観測者_YYYYMMDD_HHMMSS.csv` になるように本体で生成しています。
- **ダウンロード先が毎回聞かれる/選択制になる**  
  Chrome/Edge のダウンロード設定（「毎回保存先を確認する」）の影響です。ブラウザ設定で変更可能です。
- **位置情報が記録されない**  
  初回はブラウザに位置情報の許可が必要です。許可後に「位置取得開始」を押してください。

---
初期版のHTMLは `SPA9.06_autoname_superguard.html` から `index.html` にリネームして同梱しています。

# SPAアプリ（vibe by SPA UI 版）GitHub Pages 置き換えパック

このフォルダの中身を、**既存のGitHub Pagesリポジトリのルート直下**に上書きすれば、公開中のアプリを置き換えできます。

## 置き換え手順（Web UI）
1. GitHubで公開中のリポジトリを開く
2. `Add file > Upload files` をクリック
3. このフォルダ内の **全ファイル** をドラッグ&ドロップ（`index.html` を含む）
4. 下にスクロールして **Commit changes**
5. 数十秒後、公開URLが新バージョンに切り替わります

### 反映されない時
- URL末尾に `?v=rev2` を付けて再読み込み
- ブラウザのキャッシュ削除 / PWA再追加

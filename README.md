# SPA（しきい値超過パルス・バイブ版）

## 仕様
- **しきい値を超えたサンプル毎**に短いバイブ（既定60ms）を1回実行
- 連続してしきい値を超えている間は、**毎サンプルごと**にバイブが繰り返し発生
- しきい値未満のサンプル時はバイブなし
- 音やフラッシュとは独立に動きます（同時でもOK）

## 実装ポイント
- `window.__spaVibePulse(ms)` を追加（既定 60ms）。
- 過剰な重ねがけ防止に **最小間隔 40ms**（`window.__spaSetVibeMinGap()` で調整可）。
- 既存の `navigator.vibrate(...)` 呼び出しは本関数に置換。
- `window.emitSpaEvent({exceeded:true})` でパルスを発火（しきい値超過時）。

## 公開方法
index.html を GitHub Pages に置けばOK（manifest付き）。

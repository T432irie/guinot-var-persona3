# VAR P3 — ローカル表示（Cursor）

プレビューは **ローカル（`http://127.0.0.1:8765/`）** を既定にしてください。`index.html` は **`127.0.0.1` / `localhost`** のとき Google Tag Manager を読み込みません。

---

## A. マークダウンでサムネイルを見る

1. 左のファイル一覧から **`SITE-PREVIEW.md`** を開く。
2. **`Cmd + Shift + V`**（Windows は **`Ctrl + Shift + V`**）で **Markdown プレビュー**を開く。

### 参考キャプチャ（縮小・過去取得分）

![レイアウト参考（縮小）](varp3-preview-thumb.jpg)

※全体の高解像度 PNG は **`varp3-live-screenshot.png`**（同フォルダ）を直接開いてください。

---

## B. Simple Browser でローカル表示

1. ターミナルでプレビューサーバーを起動する。  
   - **タスクから:** `Cmd + Shift + B` → **「ローカル: プレビューサーバー (8765)」** を選ぶ  
   - **手動:**  
     `cd` してこのフォルダ（`fml`）で次を実行:

     ```bash
     python3 -m http.server 8765 --bind 127.0.0.1
     ```

2. **`Cmd + Shift + P`** → **`Simple Browser: Show`**（「シンプルブラウザ」で検索）。
3. 次の URL を貼り付けて Enter:

   **`http://127.0.0.1:8765/index.html`**

---

## 本番 URL（必要なときだけ）

公開サイト: `https://guinot.co.jp/VAR_p3/`

---

## うまくいかないとき

- **Simple Browser が見つからない:** Cursor を最新にするか、拡張機能の無効を確認。
- **接続エラー:** ポート **8765** で `python3 -m http.server` が動いているか確認。

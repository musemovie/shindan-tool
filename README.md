# プロフィールムービー診断（GitHub Pages版）

Claude.aiの「公開」機能に頼らず、自分のGitHubアカウントでホスティングするための一式です。
バージョン管理や表示のブレがなくなり、リンクプレビュー画像も自分で設定できます。

## フォルダの中身

```
index.html          ← 診断ツール本体（これだけで動作します）
assets/
  hero-cover.jpg     ← 表紙の写真
  hero-result.jpg    ← 診断結果画面の写真
  og-image.jpg       ← Instagram/ThreadsなどでリンクをシェアしたときのプレビューOGP画像
README.md            ← このファイル
```

## 公開手順（GitHub Pages）

1. **GitHubアカウントを持っていない場合**
   [github.com](https://github.com) で無料アカウントを作成

2. **新しいリポジトリを作る**
   - 右上の「+」→「New repository」
   - Repository name: 例）`profile-movie-shindan`
   - Public を選択
   - 「Create repository」

3. **このフォルダの中身をアップロード**
   - 作成したリポジトリ画面で「uploading an existing file」をクリック
   - `index.html` と `assets` フォルダをまとめてドラッグ＆ドロップ
   - 「Commit changes」

4. **GitHub Pagesを有効化**
   - リポジトリの「Settings」タブ →左メニューの「Pages」
   - 「Source」を `Deploy from a branch` に設定
   - Branch を `main`（または `master`）、フォルダを `/ (root)` にして「Save」

5. **数分待つとURLが発行されます**
   ```
   https://（あなたのGitHubユーザー名）.github.io/profile-movie-shindan/
   ```
   これがInstagram・Threadsに貼るリンクです。

## 更新したいとき

`index.html` の中身をこのファイルごと差し替えて、再度アップロード（Commit）するだけです。
反映まで通常1〜2分ほどです。Claude.aiの「公開」のようなバージョンのすり替わりは起きません。

## 独自ドメインを使いたい場合

「Settings → Pages → Custom domain」から、お持ちのドメイン（例: `shindan.musemovie.jp`）を設定できます。
その場合はドメイン管理画面でCNAMEレコードの設定も必要です。

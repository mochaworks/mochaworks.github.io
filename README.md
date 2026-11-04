# mochaworks.github.io

mochaworks のアプリの紹介・サポート・プライバシーポリシーを置く GitHub Pages サイト。

公開先: https://mochaworks.github.io/

## 構成

英語ページをルートに、日本語ページを `ja/` の下に同じ階層で置く。

```
index.html                  開発者トップ（アプリ一覧）
assets/style.css            全ページ共通のスタイル
kokomarkup/
  index.html                アプリ紹介（App Store のマーケティング URL）
  icon.png
  privacy/index.html        プライバシーポリシー（App Store のプライバシーポリシー URL）
  support/index.html        サポート（App Store のサポート URL）
ja/                         上と同じ構成の日本語ページ
```

## 新しいアプリを追加するとき

1. `kokomarkup/` と `ja/kokomarkup/` をコピーしてアプリ名のフォルダを作り、文面とアイコンを差し替える
2. `index.html` と `ja/index.html` のアプリ一覧にカードを足す

プライバシーポリシーは、アプリごとに扱うデータが違うことがあるので、アプリごとに分けて書く。

## ローカルで確認する

```bash
python3 -m http.server 8765
```

http://localhost:8765/ を開く（リンクがルートからのパスなので、ファイルを直接開くと表示が崩れる）。

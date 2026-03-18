# Markdown ➡ テーブル変換くん v3.1

MarkdownテーブルをビジュアルなHTMLテーブルに変換し、**note投稿用のPNG画像**・**HTMLコード**・**CSV**として出力できるブラウザ完結ツールです。

![version](https://img.shields.io/badge/version-3.1-6355e8) ![license](https://img.shields.io/badge/license-MIT-blue) ![type](https://img.shields.io/badge/type-standalone%20HTML-green)

---

## 概要

| 項目 | 内容 |
|------|------|
| 動作環境 | ブラウザのみ（サーバー不要） |
| ファイル構成 | HTMLファイル1枚 |
| 外部依存 | html2canvas（CDN） / Google Fonts（CDN） |
| 対象ユーザー | note・WordPress等に表を貼りたい方、福祉・教育現場の実務者 |

---

## 機能

### 入力
- Markdownテーブル貼り付け入力
- `Ctrl + Enter`（Mac: `⌘ + Enter`）でワンキー変換

### インラインMarkdown変換（v3.1追加）
セル内の装飾記法をそのまま描画します。

| 記法 | 表示 |
|------|------|
| `**太字**` | **太字** |
| `*斜体*` | *斜体* |
| `` `コード` `` | `コード` |

### スタイル調整
- 8種類のカラーテーマ（Ocean / Forest / Rose / Slate / Amber / Violet / Teal / Mono）
- フォントサイズ調整（11px〜20px）
- セル余白調整
- ストライプ（交互カラー）トグル

### 出力
| ボタン | 内容 |
|--------|------|
| ⚡ 変換して画像コピー | クリップボードにPNG画像をコピー |
| 📋 画像だけコピー | 再変換せずにPNG画像をコピー |
| 🖼️ PNGで保存 | `table.png` としてダウンロード（**v3.1追加**） |
| 📄 HTMLをコピー | `<table>` タグをクリップボードにコピー（**v3.1追加**） |
| ⬇️ CSV ダウンロード | `table.csv` としてダウンロード |

---

## 使い方

### note に表を貼る場合
1. HTMLファイルをブラウザで開く
2. 左パネルにMarkdownテーブルを貼り付け
3. テーマ・フォントを調整
4. 「🖼️ PNGで保存」でダウンロード、またはnoteの画像挿入で直接アップロード

### WordPress / HTMLサイトに貼る場合
1. 変換後「📄 HTMLをコピー」
2. サイトのHTMLエディタに貼り付け

---

## インストール

```bash
git clone https://github.com/<your-username>/md-table-converter.git
```

`MD_Table_Converter_v3.html` をブラウザで開くだけで使えます。

---

## ファイル構成

```
md-table-converter/
├── MD_Table_Converter_v3.html   # ツール本体（これだけでOK）
└── README.md
```

---

## 更新履歴

| バージョン | 内容 |
|-----------|------|
| v3.1 | セル内インラインMarkdown変換（太字・斜体・コード）対応 / PNGダウンロード追加 / HTMLコピー追加 |
| v3.0 | カラーテーマ8種・フォントサイズ調整・ストライプ切替・クリップボード画像コピー・CSV出力 |

---

## ライセンス

MIT License — 自由に使用・改変・再配布できます。

---

*AUL-DoX / [aul-dox.jp](https://aul-dox.jp)*

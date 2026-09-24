<div align="right">
<a href="../../README.md">简体中文</a> | <a href="README.en_US.md">English</a> | 日本語
</div>

<h1 align="center">hikoutai-stamp</h1>
<p align="center">航空自衛隊スタイルの写真ラベリングツール</p>

<div align="center">

[![スター](https://img.shields.io/github/stars/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=orange&label=%E3%82%B9%E3%82%BF%E3%83%BC)](https://github.com/PiggyWu981/hikoutai-stamp/stargazers)
[![最終コミット](https://img.shields.io/github/last-commit/PiggyWu981/hikoutai-stamp?style=for-the-badge&color=blue&label=%E6%9C%80%E7%B5%82%E3%82%B3%E3%83%9F%E3%83%83%E3%83%88)](https://github.com/PiggyWu981/hikoutai-stamp/commits/master)
[![オンラインデモ](https://img.shields.io/badge/%E3%83%87%E3%83%A2-4c9a42?style=for-the-badge)](https://piggywu981.github.io/hikoutai-stamp/)
[![単一ファイル](https://img.shields.io/badge/%E5%8D%95%E4%B8%80%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB-d4a84b?style=for-the-badge)](index.html)
[![依存なし](https://img.shields.io/badge/%E4%BE%9D%E5%AD%98%E3%81%AA%E3%81%97-6e7681?style=for-the-badge)](index.html)
[![Gitee ミラー](https://img.shields.io/badge/Gitee%20%E3%83%9F%E3%83%A9%E3%83%BC-c71d23?style=for-the-badge)](https://gitee.com/PiggyWu981/hikoutai-stamp)
[![ライセンス](https://img.shields.io/badge/%E3%83%A9%E3%82%A4%E3%82%BB%E3%83%B3%E3%82%B9-GPL--3.0-blue?style=for-the-badge)](../../LICENSE)

</div>

## 概要

hikoutai-stamp はブラウザ上で動作する画像ラベリングツールです。任意の写真に、航空自衛隊の公開写真と同様のレイアウトで「対象機」ラベルバーと右下のクレジットを重ね、PNG として書き出します。

処理は HTML5 Canvas を用いてブラウザ内で完結し、画像がサーバーへ送信されることはありません。操作画面は日本語です。

## 機能

- 上部ラベルと右下クレジットを個別に表示・非表示にできます
- ラベル文言は自由に編集でき、Y-9 / H-6 / Su-27 / B-52H / RC-135 の 5 種プリセットを搭載しています
- 黒地に白文字・白地に黒文字の 2 テーマを用意しています
- Canvas ベースのリアルタイムプレビューで、編集内容は即時に反映されます
- PNG 書き出しに対応。システムのシェア（Web Share）→ 直接ダウンロード → 全画面プレビューの順に保存方法を自動で切り替え、モバイルブラウザにも対応します
- クリックまたはドラッグで JPG / PNG / WebP 形式の画像を選択できます
- すべての処理はブラウザ内で行われ、サーバーは不要です
- 単一ファイル（`index.html`）実装。ビルド不要、実行時のサードパーティ依存はありません
- レスポンシブ対応で、PC・モバイルの双方で利用できます

## オンラインで使う

[https://piggywu981.github.io/hikoutai-stamp/](https://piggywu981.github.io/hikoutai-stamp/) にアクセスするだけで利用できます。インストールは不要です。

## ローカルで実行する

```bash
git clone https://github.com/PiggyWu981/hikoutai-stamp.git
cd hikoutai-stamp
python -m http.server 8000
```

ブラウザで `http://localhost:8000` にアクセスしてください。`index.html` を直接開いても動作しますが、システムのシェアなどの機能は HTTPS または localhost 環境が必要です。

## 操作方法

1. 点線部分をクリックするか、画像をページ内にドラッグして読み込みます（JPG / PNG / WebP）。
2. 左パネルで上部ラベルと右下のクレジットを編集します。プリセットボタンで機体名の文言を素早く入力できます。
3. テーマを選び、チェックボックスでラベル・クレジットの表示を切り替えます。
4. 「PNG を保存」ボタンで書き出します。

## 注意事項

> **注意**
>
> - 本ツールは航空自衛隊の公開写真のレイアウトスタイルを模したものです。学習・交流などの非公式な用途を想定しています。
> - 出力画像を公式発表資料の偽造、公衆を誤認させる目的、その他の不適切な用途に使用しないでください。
> - プリセットの機体名や「初めて確認した」といった文言はすべて例示であり、実際の出来事を示すものではありません。

## ライセンス

本リポジトリには現在ライセンスの指定がなく、LICENSE ファイルも含まれていません。

## クレジット

- フォント：[Noto Sans JP](https://fonts.google.com/noto/specimen/Noto+Sans+JP)、Noto Sans SC（Google Fonts）
- レイアウト参考：航空自衛隊の公開写真のレイアウトスタイル

## リンク

- [オンラインデモ](https://piggywu981.github.io/hikoutai-stamp/)
- [GitHub リポジトリ](https://github.com/PiggyWu981/hikoutai-stamp)
- [Gitee リポジトリ（ミラー）](https://gitee.com/PiggyWu981/hikoutai-stamp)

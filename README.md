# ProductArchive

BOOTHショップ「M.G.R Tech Creations」で販売しているデータの管理に使用するリポジトリです。
https://maguro-vrc.booth.pm/

## ドキュメントサイト

製品のマニュアルをここで公開しています。

**https://maguro-git.github.io/ProductArchive/**

| 製品 | ドキュメント |
|---|---|
| GRAY OASIS | [マニュアル](https://maguro-git.github.io/ProductArchive/gray-oasis/) |

## お問い合わせ

不具合報告・導入のご相談は、ご購入者さまを対象に BOOTH のメッセージ機能で受け付けています。
このリポジトリの Issues では受け付けていません。

---

## リポジトリ構成（管理用）

```
├─ docs/                    ドキュメントサイトのソース（Markdown）
│  ├─ index.md              製品一覧のトップページ
│  ├─ _template/            新製品追加用のひな形（サイトには出力されない）
│  └─ <製品スラッグ>/        製品ごとのマニュアル
├─ ChangeLog/               旧製品の更新履歴テキスト
├─ mkdocs.yml               サイト設定・ナビゲーション
├─ requirements.txt         ビルドに使う Python パッケージ
└─ .github/workflows/       main への push でサイトを自動更新
```

### 製品を追加する

1. `docs/_template/` を `docs/<製品スラッグ>/` にコピーする
2. 内容を書く
3. `mkdocs.yml` の `nav` にブロックを追加する
4. `docs/index.md` の製品一覧にリンクを追加する
5. `main` へ push すると自動でサイトが更新される

### ローカルでプレビューする（任意）

Python が必要です。

```bash
pip install -r requirements.txt
mkdocs serve
```

http://127.0.0.1:8000/ で確認できます。

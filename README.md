# ProductArchive

BOOTHショップ「[M.G.R Tech Creations](https://maguro-vrc.booth.pm/)」で販売している製品の、マニュアルと更新履歴を公開するリポジトリです。製品データそのものは含みません。

## ドキュメントサイト

**https://maguro-git.github.io/ProductArchive/**

| 製品 | ドキュメント |
|---|---|
| GRAY OASIS | [マニュアル](https://maguro-git.github.io/ProductArchive/gray-oasis/) |
| Japan Classroom | [マニュアル](https://maguro-git.github.io/ProductArchive/japan-classroom/) |
| SF-ROOM for VRC | [マニュアル](https://maguro-git.github.io/ProductArchive/sf-room/) |
| Apartment for VRC | [マニュアル](https://maguro-git.github.io/ProductArchive/apartment/) |
| ハンドグレネードギミック | [マニュアル](https://maguro-git.github.io/ProductArchive/hand-grenade/) |
| 無人航空機 / UAV | [マニュアル](https://maguro-git.github.io/ProductArchive/uav/) |

マニュアルが未整備の製品は、更新履歴のみ[サイト](https://maguro-git.github.io/ProductArchive/)に掲載しています。

## お問い合わせ

不具合や不明点は、各商品ページに記載の窓口までご連絡ください（商品によって窓口が異なります）。

---

## リポジトリ構成（管理用）

```
├─ docs/                    ドキュメントサイトのソース（Markdown）
│  ├─ index.md              製品一覧のトップページ
│  ├─ _template/            新製品追加用のひな形（サイトには出力されない）
│  └─ <製品スラッグ>/        製品ごとのマニュアル
├─ ChangeLog/               更新履歴の原本テキスト（旧リンク向けに残置。内容は docs/ 側と同じ）
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

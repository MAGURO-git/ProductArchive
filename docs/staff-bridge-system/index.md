# Staff Bridge System

!!! warning "開発中のため、まだ販売していません"
    Staff Bridge System は現在開発中です。このドキュメントは仕様が固まる前に先行して公開しているもので、**記載している内容・画面・機能は変更される可能性があります**。発売日は未定です。

<span class="badge badge--vrc">VRChat World</span>

<div class="product-hero" markdown>
![Staff Bridge System](images/icon.png){ .product-icon }

VRChat ワールド用のイベント運営支援ギミック一式です。テレポートメニュー・インカム（無線）・一斉メッセージ機能を簡単に導入できます。
</div>

- 商品ページ: 準備中
- 利用規約: [Staff Bridge System 利用規約（PDF）](https://drive.google.com/file/d/1Y1xBQFlrfcBY5iI4gYFHOwRgYQo4pm7a/view?usp=sharing)
- 体験ワールド: 準備中

## できること

スタッフになったプレイヤーの手元にメニューが表示され、次の操作ができます。

| 機能 | 内容 |
|---|---|
| テレポート | 登録地点および在室スタッフへの移動。お気に入り登録つき |
| インカム（無線） | 同じチャンネルのメンバーだけに聞こえる音声通話 |
| 一斉メッセージ | 全スタッフ／選択したスタッフへの定型文送信 |

あわせて、シーン側に次のものを設置できます。

| 機能 | 内容 |
|---|---|
| スタッフ限定オブジェクト | スタッフだけが見える／通れる／押せるオブジェクト |
| 在室スタッフ一覧ボード | いま入室しているスタッフ名の掲示 |
| 頭上マーカー | スタッフの頭上に表示される目印 |

## 必要環境

| 項目 | 内容 |
|---|---|
| Unity | 2022.3.22f1 |
| VRChat SDK | Worlds SDK 3.10.x 以降 |
| 日本語フォント | [tmp-fallback-fonts-jp](https://github.com/Narazaka/tmp-fallback-fonts-jp)（**必須**） |
| FukuroUdon | [FukuroUdon](https://github.com/mimyquality/FukuroUdon)（**必須**・動作確認済み 3.18.0） |
| プラットフォーム | PC 専用（Quest 実機での動作確認は行っていません） |

前提パッケージ2つは VCC / ALCOM から導入できます。詳しくは [導入](install.md) を参照してください。

!!! tip "当日のスタッフへ渡すページ"
    [スタッフの方へ](for-staff.md) は、ワールド内での操作だけを説明したページです。Unity の用語は出てきません。当日のスタッフにはこの URL を渡してください。

## ドキュメントの読み進めかた

1. [導入](install.md) — 前提パッケージの用意からセットアップまで
2. [基本の使い方](usage.md) — ワールド内での操作
3. [運用ガイド](operation.md) — イベント当日の使い方と設計の考え方
4. [設定リファレンス](reference.md) — Inspector の各項目
5. [見た目のカスタマイズ](customize.md) — テーマ・フォント
6. [トラブルシューティング](troubleshoot.md) — 症状別の対処
7. [よくある質問](faq.md)

## スタッフの付与について

スタッフの付与方法は「表示名ホワイトリスト」と「スタッフ切替スイッチ」の2通りです。スイッチは触れた本人がスタッフ ON / OFF できるため、設置場所にはご注意ください。詳しくは [運用ガイド](operation.md#staff-detection) を参照してください。

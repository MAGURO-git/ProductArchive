# Staff Bridge System

<span class="badge badge--vrc">VRChat World</span>

<div class="product-hero" markdown>
![Staff Bridge System](images/icon.png){ .product-icon }

VRChat ワールド用のイベント運営支援ギミック一式です。テレポート・インカム・一斉メッセージ・進行タイマーなどの機能を、スタッフ専用メニュー「SBSメニュー」にまとめています。
</div>

- 商品ページ: [BOOTH](https://maguro-vrc.booth.pm/items/8682451)
- 利用規約: [Staff Bridge System 利用規約（PDF）](https://drive.google.com/file/d/1udZaWP37aN14rFh5DS4WfA0J7ZAQSaax/view?usp=sharing)
- サンプルワールド: [Staff Bridge System Sample（VRChat）](https://vrchat.com/home/world/wrld_01cbbb48-44ce-4761-9baa-6f4ef87fbbfd/info)

!!! info "このドキュメントについて"
    本製品には専用の [利用規約（PDF）](https://drive.google.com/file/d/1udZaWP37aN14rFh5DS4WfA0J7ZAQSaax/view?usp=sharing) が適用されます（全体の区分は [利用規約](../terms.md) を参照）。価格などの販売条件は BOOTH の商品ページをご確認ください。

## できること

スタッフになったプレイヤーの前に専用のSBSメニューが表示されます。

- 移動と連絡 — テレポート（登録地点・在室スタッフ）／インカム／メガホン／一斉メッセージ
- 進行 — 共有タイマーと自分用タイマー／ノート（共有メモと自分用メモ）／通知ログ／入退室ログ
- 運営 — 当日スタッフの追加と削除／手元からワールド内のギミックへイベントを送るスイッチ
- 各自の調整 — 音量・UI サイズ・発話方式・通知ログの位置（再入場後も保持）

タブは並べ替えられ、使わないものは非表示にできます。

シーン側には、スタッフ限定オブジェクト（スタッフだけが見える／通れる／押せる）、在室スタッフ一覧ボード、頭上マーカーを設置できます。

イベントごとの作り込みは Unity 上の専用ウィンドウから行います。メニュー構成・テレポート先・定型文・配色テーマ・スタッフ名簿を Inspector を直接触らずに編集でき、設定の不備は診断・修復でまとめて直せます。

各機能の詳細、設定ページへの入口、できないことは [機能一覧](features.md) にまとめてあります。

## 必要環境

| 項目 | 内容 |
|---|---|
| Unity | 2022.3.22f1 |
| VRChat SDK | Worlds SDK 3.10.x 以降 |
| FukuroUdon | [FukuroUdon](https://github.com/mimyquality/FukuroUdon)（**必須**・動作確認済み 3.19.5） |
| プラットフォーム | PC 専用（Quest 実機での動作確認は行っていません） |

FukuroUdon は VCC / ALCOM から導入できます。詳しくは [導入](install.md) を参照してください。

!!! tip "当日スタッフへ渡すページ"
    [スタッフの操作ガイド](usage.md) は、ワールド内での操作だけを説明したページです。Unity の用語は出てきません。当日スタッフにはこの URL を渡してください。

## ご購入・導入前の確認事項 { #before-you-buy }

- **他の音声ギミックとの併用不可（排他仕様）**:
  防音室・個室・ボイスゾーンなど、プレイヤーの発話距離や音量を制御する他ギミックとは同時に使用できません（インカム機能か他ギミックのどちらか一方を選択してご使用ください。詳細は[運用ガイド](operation.md#incom-power)）。
- **確認済み動作規模（40人）**:
  40人規模のイベントでの運用実績があります。それを大幅に超える大規模インスタンスでの動作は未確認です。
- **PC専用・前提パッケージ**:
  PC 専用です（Quest 実機での動作確認は行っていません）。また、前提パッケージとして FukuroUdon の導入が必要です（詳細は[導入ガイド](install.md)）。
- **本番前の実機確認**:
  ワールドの構成や同時に動く他のギミックによって、想定どおりに動作しないことがあります。本番と同じワールドで一通りの機能を動かして事前にご確認ください（詳細は[本番前の確認](operation.md#pre-event-check)）。
- **利用規約・ライセンス**:
  本製品には専用の規約が適用されます。詳細は [Staff Bridge System 利用規約（PDF）](https://drive.google.com/file/d/1udZaWP37aN14rFh5DS4WfA0J7ZAQSaax/view?usp=sharing) をご確認ください。個人版（P）とチーム版（T）のライセンス区分については [よくある質問（FAQ）](faq.md) をご確認ください。

## ドキュメントの読み進めかた

あなたの役割や目的に合わせてガイドをご案内します。

<div class="guide-nav-grid">
  <a href="install/" class="guide-nav-card">
    <div class="title">ワールド制作者 <span>→</span></div>
    <div class="desc">前提パッケージの導入からセットアップ、Unity上でのカスタマイズ手順を確認できます。</div>
  </a>

  <a href="usage/" class="guide-nav-card">
    <div class="title">当日スタッフ <span>→</span></div>
    <div class="desc">ワールド内でのメニュー操作・インカム・タイマーの使い方をUnity用語なしで説明しています。</div>
  </a>

  <a href="for-developers/" class="guide-nav-card">
    <div class="title">ギミック開発者 <span>→</span></div>
    <div class="desc">自作UdonスクリプトとSBSのスイッチやスタッフ判定を連携させる方法を解説しています。</div>
  </a>

  <a href="faq/" class="guide-nav-card">
    <div class="title">購入前・ライセンス <span>→</span></div>
    <div class="desc">個人・チームライセンスの数えかたや、よくある質問を視覚的にまとめています。</div>
  </a>
</div>

## スタッフの付与について

スタッフの付与方法は「表示名ホワイトリスト」「スタッフ切替スイッチ」「メニューのスタッフ管理タブ」の3通りです。スイッチは触れた本人がスタッフ ON / OFF できるため、設置場所にはご注意ください。詳しくは [運用ガイド](operation.md#staff-detection) を参照してください。

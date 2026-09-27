# 導入

新規のワールドプロジェクトへの導入手順です。[必要環境](index.md)を確認してから始めてください。

導入手順の流れは動画でもご確認いただけます。

<https://youtu.be/DsbDUshHiPU>

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>新規プロジェクトを作成する</h3>
</div>
<div class="step-body" markdown="1">

VCC / ALCOM から VRChat ワールド用プロジェクト（Unity 2022.3.22f1 推奨）を作成します。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>必須アセットを導入する</h3>
</div>
<div class="step-body" markdown="1">

本ワールドが参照している外部アセットを導入します。

| アセット | 用途 | 入手先 |
|---|---|---|
| UdonToolkit | ギミック制御基盤 | [GitHub Releases](https://github.com/orels1/UdonToolkit/releases) |
| iwaSync3 | メディアプレイヤー | [BOOTH](https://booth.pm/ja/items/2666275) |
| Crystal Water FX | 水面シェーダー | [BOOTH](https://tsunamoo.booth.pm/items/3469326) |

!!! warning "UdonSharp の重複に注意"
    VCC環境では UdonSharp が最初から組み込まれています。旧バージョンの単体 UdonSharp パッケージを上書きインポートしないようご注意ください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>Apartment_SDK3.unitypackage をインポートする</h3>
</div>
<div class="step-body" markdown="1">

BOOTH からダウンロードした `Apartment_SDK3.unitypackage` をプロジェクトにインポートします。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>UdonToolkit の設定を確認する</h3>
</div>
<div class="step-body" markdown="1">

メニューバーの **Edit > Project Settings > UdonToolkit** を開き、必要なレイヤー設定や初期化設定が完了していることを確認します。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 5</span>
<h3>シーンを開いてアップロードする</h3>
</div>
<div class="step-body" markdown="1">

同梱のシーンファイルを開き、Play モードで動作確認後、VRChat SDK コントロールパネルからアップロードを実行します。

</div>
</div>

</div>

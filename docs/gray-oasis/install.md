# 導入

[必要環境](index.md)を確認してから始めてください。

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>VRChat ワールド用プロジェクトの作成</h3>
</div>
<div class="step-body" markdown="1">

VCC（VRChat Creator Companion）または ALCOM から、VRChat ワールド用の新規プロジェクトを作成します（Unity 2022.3.22f1）。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>必須アセット（QvPen、VizVid など）の導入</h3>
</div>
<div class="step-body" markdown="1">

ワールド内のギミックやシェーダーが参照しているため、パッケージをインポートする前に、次のアセットを導入してください。Bakery は任意です。

| アセット | 用途 | 入手先 |
|---|---|---|
| VizVid | ビデオプレイヤー | [VPMリポジトリ](https://xtlcdn.github.io/vpm/) |
| QvPen | ペンギミック | [VPMリポジトリ](https://vpm.ureishi.net/install) |
| VRC Light Volumes | アバターライティング | [GitHub](https://github.com/REDSIM/VRCLightVolumes) |
| Visitors Information Board | 入退室ログ表示 | [BOOTH](https://booth.pm/ja/items/5403376) |
| Mochies-Unity-Shaders | 水・エフェクト用シェーダー | [GitHub](https://github.com/MochiesCode/Mochies-Unity-Shaders) |
| Bakery - GPU Lightmapper | ライティングベイク（任意） | [Unity Asset Store](https://assetstore.unity.com/packages/tools/level-design/bakery-gpu-lightmapper-122218?locale=ja-JP) |

!!! tip "Bakery を導入していない場合"
    Bakery を導入していない場合は、同じパッケージに入っているビルトインライトマッパー版のシーンを使用できます。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>取り出した unitypackage のインポート</h3>
</div>
<div class="step-body" markdown="1">

1. 購入データの `GRAY_OASIS_v1.2.1_展開方法.pdf` の手順で、2つの zip から `GRAY_OASIS_v1.2.1.unitypackage` を取り出します。
2. 取り出した `GRAY_OASIS_v1.2.1.unitypackage` を、プロジェクトにインポートします。

シーンとテクスチャは、すべてこのパッケージに入っています。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>シーンの選択（Bakery 版 / ビルトインライトマッパー版）</h3>
</div>
<div class="step-body" markdown="1">

**Project** ウィンドウから次のシーンを開きます。

- Bakery 版: `Assets/MGR/GrayOasis/GrayOasis.unity`
- ビルトインライトマッパー版: `Assets/MGR/GrayOasis/GrayOasis_builtinLightmapper.unity`

!!! note "ビルトインライトマッパー版は、導入後に再ベイクします"
    このパッケージには、Bakery 版とビルトインライトマッパー版の2つのシーンが入っています。モデルの .meta ファイルは2つのシーンで共通のため、ライトマップ用の UV がずれて見えることがあります。ビルトインライトマッパー版は、導入後に一度ライトを再ベイクした状態が、意図した見た目です。[ライティングの再ベイク](customize.md)の手順で、再ベイクしてください。Bakery 版は、再ベイクが不要です。

![シーンの場所](images/scene-location.png)

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 5</span>
<h3>動作確認とアップロード</h3>
</div>
<div class="step-body" markdown="1">

1. Unity の Play モード（ClientSim）に入り、スポーン位置、ライティング、ギミックの動作を確認します。
2. 問題がなければ、VRChat SDK コントロールパネルの **Builder** タブで、ワールドのタイトル、説明文、サムネイル画像を設定します。
3. **Build and Upload** を実行します。

</div>
</div>

</div>

# 導入

[必要環境](index.md)を確認してから始めてください。

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>プロジェクトを作成する</h3>
</div>
<div class="step-body" markdown="1">

VCC（VRChat Creator Companion）または ALCOM から、VRChat ワールド用の新規プロジェクトを作成します（Unity 2022.3.22f1）。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>必須アセットを導入する</h3>
</div>
<div class="step-body" markdown="1">

ワールド内のギミックやシェーダーが参照しているため、パッケージをインポートする前にすべて導入してください。

| アセット | 用途 | 入手先 |
|---|---|---|
| VizVid | ビデオプレイヤー | [VPMリポジトリ](https://xtlcdn.github.io/vpm/) |
| QvPen | ペンギミック | [VPMリポジトリ](https://vpm.ureishi.net/install) |
| VRC Light Volumes | アバターライティング | [GitHub](https://github.com/REDSIM/VRCLightVolumes) |
| Visitors Information Board | 入退室ログ表示 | [BOOTH](https://booth.pm/ja/items/5403376) |
| Mochies-Unity-Shaders | 水・エフェクト用シェーダー | [GitHub](https://github.com/MochiesCode/Mochies-Unity-Shaders) |
| Bakery - GPU Lightmapper | ライティングベイク（任意） | [Unity Asset Store](https://assetstore.unity.com/packages/tools/level-design/bakery-gpu-lightmapper-122218?locale=ja-JP) |

!!! tip "Bakery をお持ちでない場合"
    Bakery をお持ちでない場合は、同じパッケージに入っているビルトインライトマッパー版のシーンを使用できます。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>unitypackage をインポートする</h3>
</div>
<div class="step-body" markdown="1">

1. 購入データの `GRAY_OASIS_v1.2.1_part1.zip` と `GRAY_OASIS_v1.2.1_part2.zip` を、同じフォルダに展開します。`GRAY_OASIS_v1.2.1.unitypackage.001` と `.002` ができます。
2. 展開したフォルダで、エクスプローラーのアドレスバーに `cmd` と入力して **Enter** を押し、コマンドプロンプトを開きます。
3. 次のコマンドを実行して、2つのファイルを1つにまとめます。

    ```
    copy /b GRAY_OASIS_v1.2.1.unitypackage.001 + GRAY_OASIS_v1.2.1.unitypackage.002 GRAY_OASIS_v1.2.1.unitypackage
    ```

4. できた `GRAY_OASIS_v1.2.1.unitypackage` を、プロジェクトにインポートします。

シーンとテクスチャは、すべてこのパッケージに入っています。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>シーンを開く</h3>
</div>
<div class="step-body" markdown="1">

**Project** ウィンドウから次のシーンを開きます。

- Bakery版: `Assets/MGR/GrayOasis/GrayOasis.unity`
- ビルトイン版: `Assets/MGR/GrayOasis/GrayOasis_builtinLightmapper.unity`

!!! note "ビルトイン版は、導入後に再ベイクします"
    ビルトイン版のライトマップは、Bakery が入った環境でベイクしています。モデルのライトマップ用 UV は Bakery の有無で変わるため、Bakery が入っていない環境では、一部のモデルでライトマップがずれて見えます。導入後に、[ライティングの再ベイク](customize.md)の手順で、再ベイクしてください。Bakery 版のシーンは、再ベイクが不要です。

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

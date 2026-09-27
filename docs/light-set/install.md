# 導入

Unity プロジェクトへのインポートおよびシーンへの配置手順です。[仕様](index.md)を確認してから始めてください。

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>unitypackage をインポートする</h3>
</div>
<div class="step-body" markdown="1">

BOOTH からダウンロードした unitypackage を Unity プロジェクトへインポートします。
`Assets/` 配下にモデル・テクスチャ・Prefab が展開されます。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>照明 Prefab をシーンに配置する</h3>
</div>
<div class="step-body" markdown="1">

Project ウィンドウからお好みの照明 Prefab を Scene または Hierarchy にドラッグ＆ドロップして配置します。
天井面や壁面に合わせて Transform（Position / Rotation）を調整してください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>ライトの光量・色を調整する</h3>
</div>
<div class="step-body" markdown="1">

Prefab 内に含まれる `Light` コンポーネントを選択し、Inspector からお好みの設定に変更します。

- **Mode**: `Baked`（推奨）または `Mixed`
- **Color**: 昼光色、温白色、電球色など部屋の雰囲気に合わせて調整
- **Intensity**: 空間の明るさに応じた光量調整
- **Range / Spot Angle**: 光が届く範囲や照射角度の調整

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>ライティングをベイクする</h3>
</div>
<div class="step-body" markdown="1">

配置した照明オブジェクトを Static（Contribute GI / Lightmap Static）に設定し、Unity 標準のライトマッパーまたは Bakery でライティングをベイクします。

</div>
</div>

</div>

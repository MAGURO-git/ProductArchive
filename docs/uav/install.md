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
`Assets/` 配下にモデル・テクスチャ・Prefab・アニメーションクリップが展開されます。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>Prefab をシーンに配置する</h3>
</div>
<div class="step-body" markdown="1">

Project ウィンドウから UAV の Prefab を Scene または Hierarchy にドラッグ＆ドロップして配置します。
お好みの位置や向きに Transform を調整してください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>アニメーションを設定・再生する</h3>
</div>
<div class="step-body" markdown="1">

機体にはプロペラ回転やランディングギア（着陸脚）格納のアニメーションが含まれています。

- **自動ループ再生**:
  同梱の Animator Controller を Prefab の Animator コンポーネントに割り当てておくことで、Play モード時に自動的にアニメーションがループ再生されます。
- **Timeline での制御**:
  Unity Timeline やアニメーションイベントから再生タイミングを制御することも可能です。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>コライダーの追加（ワールド用途）</h3>
</div>
<div class="step-body" markdown="1">

VRChat ワールドに設置してプレイヤーが乗ったり触れたりできるようにする場合は、機体の形状に合わせて `Box Collider` や `Mesh Collider`（Convex 推奨）を適宜追加してください。

</div>
</div>

</div>

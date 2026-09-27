# 導入

Modular Avatar を使用したアバターへの導入手順です。[必要環境](index.md)を確認してから始めてください。

同じ手順を動画でもご確認いただけます。

<https://youtu.be/VFBRsUQBYxI>

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>必須アセットを導入する</h3>
</div>
<div class="step-body" markdown="1">

VCC / ALCOM から次の2つのパッケージをアバタープロジェクトに追加します。

- [Modular Avatar](https://modular-avatar.nadena.dev/ja)
- [lilToon](https://lilxyzw.github.io/lilToon/)

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>Prefab をアバター直下に配置する</h3>
</div>
<div class="step-body" markdown="1">

Project ウィンドウから `MA_GranadeGimmick` Prefab を、アバターのルートオブジェクト直下にドラッグ＆ドロップして配置します。

![アバター直下に配置した状態](images/place-prefab.png)

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>パーティクルの発生位置を調整する</h3>
</div>
<div class="step-body" markdown="1">

配置した **`MA_GranadeGimmick` 自体の Transform** を動かして、手榴弾のエフェクトが出る位置をアバターの体格に合わせます。子オブジェクトではなく、この Prefab のルートを動かしてください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>パラメータ名をコピーする</h3>
</div>
<div class="step-body" markdown="1">

配置した `MA_GranadeGimmick` を選択し、Inspector の MA Parameters にある **PBプレフィックス** のパラメータ名をクリップボードにコピーします。

![MA Parameters](images/ma-parameters.png)

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 5</span>
<h3>発火させたい PhysBone を選ぶ</h3>
</div>
<div class="step-body" markdown="1">

掴んで固定したときにギミックを動かしたい PhysBone（スカート、リボン、アホ毛など）を、Hierarchy で選択します。

![PhysBone を選択](images/select-physbone.png)

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 6</span>
<h3>PhysBone のパラメータを設定する</h3>
</div>
<div class="step-body" markdown="1">

選択した PhysBone コンポーネントで、次の3項目を設定します。

| 場所 | 項目 | 設定値 |
|---|---|---|
| **Grab & Pose** | Allow Grabbing | **True**（チェックを入れる） |
| **Grab & Pose** | Allow Posing | **True**（チェックを入れる） |
| **Options** | Parameter | **STEP 4 でコピーしたパラメータ名を貼り付け** |

![PhysBone の設定](images/physbone-settings.png)

これで設定は完了です。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 7</span>
<h3>Play モードで動作を確認する</h3>
</div>
<div class="step-body" markdown="1">

1. **セーフティを解除する**:
   アバターのエクスプレッションメニューから `HandGrenade_ON` を ON にします（誤操作防止のため初期状態は OFF です）。
   ![メニューのセーフティ](images/menu-safety.png)

2. **PhysBone を掴んで固定する**:
   Game ビューで設定した PhysBone をマウスの右クリックで掴み、そのまま左クリックして固定（Posing）します。固定と同時に手榴弾の音とエフェクトが発生すれば成功です。

!!! warning "周囲の環境に配慮してください"
    音と光のエフェクトが発生します。周囲の迷惑にならない範囲でご使用ください。使い終わったらメニューの `HandGrenade_ON` を OFF に戻しておくことを推奨します。

</div>
</div>

</div>

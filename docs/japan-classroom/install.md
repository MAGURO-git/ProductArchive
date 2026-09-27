# 導入

新規のワールドプロジェクトへの導入手順です。[必要環境](index.md)を確認してから始めてください。

<div class="step-container" markdown="1">

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 1</span>
<h3>分割アーカイブを解凍・結合する</h3>
</div>
<div class="step-body" markdown="1">

BOOTH からダウンロードした分割ファイルを結合して `JapanClassroom.unitypackage` を生成します。

1. `JapanClassroom.part1.zip` を解凍します。
2. 解凍して現れた `JapanClassroom.part1.exe` を、ダウンロードした `part2.rar` / `part3.rar` と**同じフォルダに置きます**。
3. `JapanClassroom.part1.exe` をダブルクリックして実行すると、自動的に結合され `JapanClassroom.unitypackage` が生成されます。

!!! tip "Mac や Linux で解凍する場合"
    `.exe` が実行できない環境では、The Unarchiver などの分割 RAR 対応解凍ソフトを使用して `part1.rar` から解凍してください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 2</span>
<h3>プロジェクト作成と必須アセットの導入</h3>
</div>
<div class="step-body" markdown="1">

VCC / ALCOM から VRChat ワールド用の新規プロジェクトを作成（Unity 2022.3.22f1 推奨）し、次の必須アセットを導入します。

| アセット | 用途 | 入手先 |
|---|---|---|
| VizVid | ビデオプレイヤー | [GitHub (VPM)](https://github.com/JLChnToZ/VVMW) |
| KineL Player Counter | 入室人数カウント | [nirila's VPM Repository](https://vpm.niri.la/howtouse/) |
| VRChat向けUI集＋スイッチ | ワールド操作UI | [BOOTH](https://kakushop.booth.pm/items/5345171) |

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 3</span>
<h3>unitypackage をインポートする</h3>
</div>
<div class="step-body" markdown="1">

STEP 1 で生成した `JapanClassroom.unitypackage` をプロジェクトにインポートします。

!!! note "追加テクスチャについて（要確認）"
    もし購入データ内に「テクスチャのダウンロードリンク.txt」等の案内が含まれている場合は、記載の指示に従って追加テクスチャをインポートしてください。

</div>
</div>

<div class="step-item" markdown="1">
<div class="step-item-head">
<span class="step-num">STEP 4</span>
<h3>シーンを開いてアップロードする</h3>
</div>
<div class="step-body" markdown="1">

`Assets/MGR/JapanClassroom/Scenes/` 配下に3つのシーンが用意されています。

- `JapanClassroom_Asa.unity`（朝シーン）
- `JapanClassroom_Yu.unity`（夕方シーン）
- `JapanClassroom_Yoru.unity`（夜シーン）

アップロードしたい時間帯のシーンをダブルクリックして開き、VRChat SDK コントロールパネルの「Builder」タブから「Build and Upload」を実行します。

</div>
</div>

</div>

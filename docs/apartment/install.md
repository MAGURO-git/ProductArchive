# 導入

!!! warning "この手順は SDK3 対応時点（2022年9月）のものです"
    当時のバージョンを前提に、unitypackage を手動で順に入れる形になっています。現在の VRChat SDK や VCC / ALCOM を使った導入とは手順が異なります。現行環境での動作確認は行っていません。

    現行のバージョンで導入した場合、ギミックが動作しないなどの差異が出ることがあります。その場合の設定のやり直しや差し替えは、購入者さまご自身での対応をお願いします。

導入手順の動画を公開しています。画面の流れはこちらが分かりやすいです。

<https://youtu.be/DsbDUshHiPU>

## 手順の概要

1. 新しいプロジェクトを作成する
2. 下記のアセットを**上から順に**インポートする
3. `Apartment_SDK3.unitypackage` をインポートする
4. UdonToolkit を設定する（Edit ＞ Project Settings から）
5. シーンを開き、ワールド名・キャパシティ・サムネイルを設定してアップロードする

## インポートするアセット

| 順 | アセット | 入手先 |
|---|---|---|
| 1 | VRCSDK3-WORLD-2022.08.29.20.48_Public | <https://vrchat.com/home/download> |
| 2 | UdonSharp v0.20.3 | [vrchat-community/UdonSharp](https://github.com/vrchat-community/UdonSharp/releases) |
| 3 | UdonToolkit | [orels1/UdonToolkit](https://github.com/orels1/UdonToolkit/releases) |
| 4 | 【VRC向け】iwaSync3 メディアプレイヤー | [BOOTH](https://booth.pm/ja/items/2666275) |
| 5 | Crystal Water FX - Flowing Water Shader | [BOOTH](https://tsunamoo.booth.pm/items/3469326) |

同梱の unitypackage とあわせて、利用規約のテキストファイルも入っています。

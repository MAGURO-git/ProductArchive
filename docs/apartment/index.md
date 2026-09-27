# Apartment for VRC

<span class="badge badge--vrc">VRChat World</span>

<div class="product-hero" markdown>
モダンで落ち着いた高級マンション・アパートの一室をイメージした VRChat 向けワールドです。リビング、ベッドルーム、バスルームを備え、購入者を含む2名までデータを共有して制作できる「シェア可能ライセンス」に対応しています。
</div>

- 商品ページ: [BOOTH](https://maguro-vrc.booth.pm/items/1509768)

## サンプルワールド

部屋の広さや家具の質感、落ち着いた照明の雰囲気を VRChat 内で体験できます。

- [Apartment for VRC（VRChat）](https://vrchat.com/home/world/wrld_fbc99e97-1a85-4f5d-b3e3-80d800823322)

## ギミック

ワールド内に設定されている主なギミック・設備です。特記のないものは商品データにあらかじめ組み込まれています。

- [iwaSync3](https://booth.pm/ja/items/2666275) — 別途導入が必要
- [Crystal Water FX](https://tsunamoo.booth.pm/items/3469326) — 別途導入が必要
- [UdonToolkit](https://github.com/orels1/UdonToolkit/releases) — 別途導入が必要
- 個別照明スイッチ（リビング、ベッドルーム、バスルーム）
- 玄関ドア開閉
- 各種ミラー
- 環境BGM

操作仕様の詳細は [ギミック一覧](gimmicks.md) を参照してください。

## 必要環境・制作環境

| 項目 | 内容 |
|---|---|
| 制作時 Unity | Unity 2019.4.31f1（制作・SDK3対応当時） |
| 制作時 SDK | Worlds SDK 3（当時のスタンドアロン版 / UdonSharp v0.20.3） |
| ワールド容量 | 約85MB |
| 必須アセット | UdonToolkit / iwaSync3 / Crystal Water FX（詳細は[導入](install.md)） |
| プラットフォーム | PC 専用（Quest 実機での動作確認は行っていません） |

## ご購入・導入前の確認事項

- **旧環境制作・ギミックの動作保証について**:
  本商品は2022年当時の旧環境（Unity 2019 / スタンドアロン版SDK3 / UdonSharp v0.20）で制作された製品です。現在の VCC 環境（Unity 2022 / 最新Worlds SDK）では、パッケージ仕様の違いや UdonToolkit のバージョン差異により、一部ギミックが正常に動作しない可能性があります。現行環境でのギミック動作は保証しておらず、特別な理由がない限り最新SDKへの追従アップデートは行っていません。
- **2名までの制作データ共有に対応**:
  購入者本人を含む「2名まで」であれば、同じデータを共有して共同制作できます（追加購入不要）。3名以上のチームで共有する場合は、人数分の購入が必要です。
- **同梱再配布アセットの制限**:
  本製品には他の制作者様によるテクスチャ・BGM・効果音が含まれています。これらの再配布素材は改変できません。また、一部の素材は R-18/R-18G コンテンツでの利用が認められていません（詳細は[使用アセット](credits.md)）。
- **利用規約**:
  本製品には専用の規約が適用されます。詳細は [Apartment for VRC 利用規約](terms.md) をご確認ください。

## ドキュメント一覧

- [導入ガイド](install.md) — 必須アセットの導入順序、unitypackage のインポートとアップロード手順
- [ギミック一覧](gimmicks.md) — メディアプレイヤーや照明スイッチ、水面エフェクトの仕様
- [トラブルシューティング](troubleshoot.md) — VCC環境でのコンパイルエラーや水シェーダーの解決策
- [使用アセット](credits.md) — 同梱再配布アセットの一覧と利用条件
- [利用規約](terms.md) — 本製品専用の利用規約全文
- [更新履歴](changelog.md) — バージョン履歴

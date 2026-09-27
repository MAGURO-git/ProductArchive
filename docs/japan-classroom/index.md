# Japan Classroom

<span class="badge badge--vrc">VRChat World</span>

<div class="product-hero" markdown>
日本の高校の教室をイメージした、ノスタルジックな VRChat 向けワールドです。窓から差し込む自然光や黒板・机の質感、学校ならではの触れる小道具ギミックがあらかじめ設定されています。朝・夕・夜の3つの独立したシーンを同梱しています。
</div>

- 商品ページ: [BOOTH](https://maguro-vrc.booth.pm/items/5464478)

## サンプルワールド

時間帯によって異なる光と空気感を VRChat 内で体験できます。

- [朝シーン（ASA）](https://vrchat.com/home/world/wrld_9fc456f8-753a-4a23-ac02-cbb1f4650fdd) — 澄んだ青空と明るい日差しが差し込む朝の教室
- [夕方シーン（YU）](https://vrchat.com/home/world/wrld_b3bc231e-bee7-400a-98f9-f31b45a05919) — 情緒的な西日と窓からのライトシャフト（光条）が印象的な夕方の教室
- [夜シーン（YORU）](https://vrchat.com/home/world/wrld_6b904d32-3355-49b8-a694-74389c4dcecc) — 天井の蛍光灯と外の暗闇がリアルな、静まり返った放課後の教室

## ギミック

教室内に設定されている主なギミックです。特記のないものは商品データにあらかじめ組み込まれています。

- [VizVid](https://github.com/JLChnToZ/VVMW) — 別途導入が必要
- [KineL Player Counter](https://vpm.niri.la/howtouse/) — 別途導入が必要
- [【無料】VRChat向けUI集＋スイッチ](https://kakushop.booth.pm/items/5345171) — 別途導入が必要
- [【無料】オブジェクトリセットギミック](https://booth.pm/ja/items/4490020)
- [【無料】VRChat Udon 入退室ログアセット](https://booth.pm/ja/items/2683599)
- [Smart Mirror](https://booth.pm/ja/items/3292060)
- [VRCPlayersOnlyMirror](https://booth.pm/ja/items/2685621)
- [アズキド時計](https://booth.pm/ja/items/2225650)
- つかめる小道具（黒板消し、ほうき・ちりとり、机・椅子、定規等）
- 環境演出（1時間ごとの学校チャイム、エアコン・扇風機の稼働音）

操作場所や同期仕様の詳細は [ギミック一覧](gimmicks.md) を参照してください。

## 必要環境・制作環境

| 項目 | 内容 |
|---|---|
| 制作時 Unity | Unity 2022.3.6f1（制作当時） |
| 制作時 SDK | Worlds SDK 3（2024年2月当時） |
| ワールド容量 | 約75〜80MB |
| 必須アセット | VizVid / KineL Player Counter / VRChat向けUI集＋スイッチ（詳細は[導入](install.md)） |
| プラットフォーム | PC 専用（Quest 実機での動作確認は行っていません） |

## ご購入・導入前の確認事項

- **ギミックの動作保証・互換性について**:
  本商品は2024年2月時点の環境（Unity 2022.3.6f1 / 当時のSDK3）で制作された製品です。制作当時の環境では動作確認を行っていますが、その後の最新 Worlds SDK 環境での網羅的なギミック動作確認は行っておらず、最新環境での動作は保証していません。また、特別な理由がない限り最新SDKへの継続的な追従アップデートは行っていません。
- **分割アーカイブの解凍**:
  BOOTH のファイルサイズ制限のため、データは3分割（`part1.zip`, `part2.rar`, `part3.rar`）されています。解凍した `part1.exe` を同一フォルダで実行して結合します。
- **シーンごとのアップロード**:
  朝・夕・夜は別々のシーンとして分かれています。アップロードしたい時間帯のシーンを開いてビルドしてください。
- **利用規約**:
  ワールドの利用条件は [利用規約](../terms.md) に準拠します。

## ドキュメント一覧

- [導入ガイド](install.md) — 分割ファイルの結合手順、必須アセットの導入からアップロードまで
- [ギミック一覧](gimmicks.md) — 黒板消しやほうき、操作パネル、チャイムの仕様
- [夕方シーンの光調整](customize.md) — 西日の角度やライトシャフトの調整方法
- [トラブルシューティング](troubleshoot.md) — 分割解凍のエラー、ピンクマテリアル、音が鳴らない等の解決策
- [使用アセット](credits.md) — 同梱・使用アセットのクレジット
- [更新履歴](changelog.md) — バージョン履歴

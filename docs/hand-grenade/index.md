# ハンドグレネードギミック

<span class="badge badge--vrc">VRChat Avatar</span>

<div class="product-hero" markdown>
PhysBone（スカートやアホ毛など）を掴んで固定（Pose）すると、手榴弾の爆発エフェクトと迫力のサウンドが発生するアバター用ギミックです。Modular Avatar に対応しており、非破壊で簡単に導入できます。
</div>

- 商品ページ: [BOOTH](https://maguro-vrc.booth.pm/items/6215675)
- 紹介・導入動画: [YouTube](https://youtu.be/VFBRsUQBYxI)

## ギミックの特徴

- **直感的な発火アクション** — スカートやリボン、髪など、指定した部位の PhysBone を掴んで固定するだけで手榴弾のエフェクトが発生します。
- **Modular Avatar 完全対応** — 元のアバターの Animator やメニュー階層を一切改変せず、Prefab を配置してパラメータを指定するだけで自動結合されます。
- **誤操作防止のセーフティ** — メニューの `HandGrenade_ON` トグルで機能を一時停止できるため、意図しないタイミングでの誤発火を防げます。
- **迫力のエフェクト＆SE** — 臨場感のある爆発パーティクル、煙、閃光、専用サウンドをパッケージに同梱しています。

## 必要環境・仕様

| 項目 | 内容 |
|---|---|
| Unity | 2022.3.22f1 |
| VRChat SDK | Avatars SDK 3.x |
| 容量 | 約46MB |
| 必須アセット | [Modular Avatar](https://modular-avatar.nadena.dev/ja) ／ [lilToon](https://lilxyzw.github.io/lilToon/) |
| 備考 | 3Dモデル・パーティクル・サウンドを同梱。衣装・アバター本体は付属しません |

## ご使用前の確認事項

- **周囲への配慮**:
  音と光のエフェクトが発生します。周囲の迷惑にならない範囲で、状況を確認してからご使用ください。
- **連続発火時の同期**:
  PhysBone の固定状態を検知して同期するため、通信環境や連続操作によって他者視点の見た目が同期しないことがあります。
- **利用規約**:
  本ギミックの利用条件は [利用規約](../terms.md) に準拠します。

## ドキュメント一覧

- [導入ガイド](install.md) — Modular Avatar を使ったアバターへの配置・PhysBone設定手順
- [カスタマイズ](customize.md) — 爆発の発生位置・角度の調整、音量や別部位への割り当て方法
- [トラブルシューティング](troubleshoot.md) — 固定しても発火しない、メニューが出ない等の解決策
- [更新履歴](changelog.md) — バージョン履歴

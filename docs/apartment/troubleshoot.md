# トラブルシューティング

Apartment for VRC の導入・運用時によくある問題と解決策です。

---

## 最新の VCC 環境でコンパイルエラー（赤字）が出る

**原因**: 旧バージョンの UdonSharp やパッケージが競合している可能性があります。

**対処**:
1. VCC の Manage Project から、UdonSharp や ClientSim が最新の公式バージョンに更新されているか確認してください。
2. インポート時に `Assets/UdonSharp/` などの古いフォルダが重複して展開されている場合は、バックアップをとった上で古いスクリプトフォルダを整理してください。

---

## バスタブの水がピンク色になる・透明にならない

**原因**: `Crystal Water FX` シェーダーがプロジェクトに未インポート、またはシェーダーエラーが発生しています。

**対処**:
1. [Crystal Water FX](https://tsunamoo.booth.pm/items/3469326) がプロジェクトに正しくインポートされているか確認してください。
2. マテリアルを選択し、Inspector で指定されている Shader を確認・再設定してください。

---

## 部屋のライティングが不自然（暗すぎる / 明るすぎる）

**原因**: Unity 2022 への移行に伴い、カラースペースや環境光の設定が変化した可能性があります。

**対処**:
1. **Edit > Project Settings > Player** で、Color Space が「Linear」になっているか確認してください。
2. **Window > Rendering > Lighting** を開き、「Generate Lighting」を実行してライトマップを再ベイクしてください。

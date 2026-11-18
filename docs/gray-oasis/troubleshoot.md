# トラブルシューティング

GRAY OASIS の導入や改変時に発生しやすい問題と、その解決策をまとめています。

---

## マテリアルがピンク色になる

**原因**: 必要なシェーダーがインポートされていません。

**対処**: [導入](install.md)の手順に従い、必須アセット（`Mochies-Unity-Shaders`）をインポートします。多くの場合、これでマテリアルが正常に表示されます。

---

## 部屋の中が真っ暗になる・影が異常に濃い

**原因**: Bakery を導入していない環境で、Bakery版のシーンを開いている可能性があります。

**対処**:
1. Bakery を導入していない場合は、`Assets/MGR/GrayOasis/GrayOasis_builtinLightmapper.unity`（ビルトインライトマッパー版シーン）を開きます。
2. それでも暗い場合は、**Window > Rendering > Lighting** から **Generate Lighting** を実行してライトマップを再生成します。

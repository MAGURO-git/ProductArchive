# この画像の出どころ

`menu-*.png` は**手で撮らない。差し替えもしない。**

製品リポジトリ（`vrc-products`）の画像プールから配られたものです。

```
cd vrc-products-world
uloop execute-dynamic-code --code-file ../mockups/scripts/shoot_all.cs   # 撮る
python ../mockups/scripts/distribute_shots.py                           # ここへ配る
```

ここで直接差し替えると、次に配ったときに上書きされて消えます。
UIが変わったら製品リポジトリ側で撮り直してください。

詳細は `vrc-products/mockups/shots/README.md`。

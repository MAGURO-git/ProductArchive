# 見た目のカスタマイズ

メニューの配色とフォントは、セットアップウィンドウの **カスタマイズ > テーマ・フォント** ページから変更します。

![テーマ・フォントページ](images/edit-theme.png)

テーマを選ぶと、その場でミニプレビューが更新されます。下の帯は左から 背景／面／ボタン／選択／発話／退出／文字／補足 の役割色です。

## テーマを選ぶ

同梱プリセットは9種類です。選択すると、実機と同じ比率のミニプレビューで配色を確認できます。

下の表の配色見本は、左から 背景／面／ボタン／選択／文字 です（セットアップウィンドウに出る見本と同じ並び順）。「選択」はタブや現在地のハイライトに使う色です。

### 暗色

<div class="theme-table" markdown>

| テーマ | 配色 | 特徴 |
|---|---|---|
| コントロールルーム（既定） | <span class="sw"><i style="background:#0D1119"></i><i style="background:#161D2B"></i><i style="background:#222C3F"></i><i style="background:#0062F5"></i><i style="background:#EFF3FA"></i></span> | 紺の背景と青のアクセント |
| バックステージ（炭黒×イエロー） | <span class="sw"><i style="background:#131211"></i><i style="background:#1E1C19"></i><i style="background:#262421"></i><i style="background:#FFC933"></i><i style="background:#F7F5F0"></i></span> | 炭黒の背景と黄色のアクセント |
| トワイライト（藍紫） | <span class="sw"><i style="background:#181729"></i><i style="background:#232138"></i><i style="background:#302D4B"></i><i style="background:#A99BE8"></i><i style="background:#F2F0FA"></i></span> | 藍紫の背景と薄紫のアクセント |
| ランタン（暖色） | <span class="sw"><i style="background:#1C1613"></i><i style="background:#281F1A"></i><i style="background:#362A22"></i><i style="background:#F0913D"></i><i style="background:#F7F0E8"></i></span> | 暗い茶色の背景とオレンジのアクセント |
| オーシャン（深青×シアン） | <span class="sw"><i style="background:#101820"></i><i style="background:#182430"></i><i style="background:#24333F"></i><i style="background:#3EC6DE"></i><i style="background:#EDF4F8"></i></span> | 深い青の背景とシアンのアクセント |
| いちごショコラ（暗色） | <span class="sw"><i style="background:#241318"></i><i style="background:#311C24"></i><i style="background:#402731"></i><i style="background:#F291B4"></i><i style="background:#FAF2F0"></i></span> | 暗い赤茶の背景とピンクのアクセント |
| グラファイト（無彩色） | <span class="sw"><i style="background:#141518"></i><i style="background:#1F2126"></i><i style="background:#2A2D33"></i><i style="background:#E8EAEE"></i><i style="background:#EDEFF2"></i></span> | 黒の背景と白のアクセント |
| カラーユニバーサル | <span class="sw"><i style="background:#12151A"></i><i style="background:#1B2028"></i><i style="background:#2A3038"></i><i style="background:#E9EDF2"></i><i style="background:#EDF1F6"></i></span> | 発話=青・OFF=橙 |

</div>

### 明色

<div class="theme-table" markdown>

| テーマ | 配色 | 特徴 |
|---|---|---|
| ストロベリークリーム（明色） | <span class="sw"><i style="background:#F6EDE6"></i><i style="background:#FBF6F1"></i><i style="background:#EBDBD2"></i><i style="background:#D96A93"></i><i style="background:#3A2E2C"></i></span> | クリーム色の背景とピンクのアクセント |

</div>

## 配色を自分で決める（カスタム）

テーマ一覧の「カスタム（色を自分で決める）」を選ぶと、役割色12色を個別に編集できます。プリセットの色を一部だけ変えることもできます。

各色の用途は、どのテーマでも共通です。

| 役割 | 用途 |
|---|---|
| 背景 / 面 / ボタン | 地の色 |
| 選択（アクセント） | 選択中・現在地・タブ |
| 発話（Success 系） | 送信・確定 |
| 退出（Danger 系） | OFF・退出 |
| 本文 / 見出し | 文字色 |

発話ボタンと退出ボタンは「ボタンの地色 ＋ 左端の意味色の帯 ＋ 意味色の文字」で構成されます。送信は緑系・退出は赤系という色分けは、カラーユニバーサル（青 × 橙）を除いて共通です。

## フォントを差し替える { #font }

出荷テキストは軽量な Empty SDF を参照し、VRChatではクライアント内蔵の日本語フォントへフォールバックして表示されます。Unity Editorでは、前提パッケージの日本語フォントをセットアップがフォールバックへ設定します。指定なしのままで使えます。

差し替えたい場合は、同じ画面の「フォント（任意）」に TMP フォントアセットを指定すると、生成されるテキストにそのフォントが使われます。色テーマとは独立した設定なので、どのテーマとも組み合わせられます。

!!! warning "レイアウトは既定フォント前提です"
    メニューの余白と文字サイズは既定フォントに合わせて詰めてあります。差し替えた場合の見た目は保証しません。文字幅や縦メトリクスが違うフォントでは、文字のはみ出しや上下のずれが出ることがあります。差し替えるときは実機で表示を確認してください。

## 生成済みのメニューに適用する

「シーンのメニューへ適用（色とフォントのみ）」 を押すと、すでに配置してあるメニューを作り直さずに塗り替えます。テレポート先・参照・各種設定はそのまま保持されます。

これから新しく生成する場合は、このボタンは不要です（選択中のテーマで生成されます）。

!!! warning "プレイモード中は使えません"
    プレイ中の変更はプレイ終了時に元へ戻ってしまうため、ボタンは無効化されます。プレイモードを終了してから実行してください。

!!! note "手塗りした色について"
    塗り替えはテーマの色と一致する要素だけを対象にします。生成時と別の色を手動で塗った要素は変更されません。

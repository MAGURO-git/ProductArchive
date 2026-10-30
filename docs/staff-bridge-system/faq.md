# よくある質問

## 導入について

必要環境・対応規模・他の音声ギミックとの併用は[製品概要](index.md#before-you-buy)、前提パッケージとセットアップは[導入](install.md)を参照してください。

## 機能について

- できること・制限を知る：[機能一覧](features.md)
- ワールド内で操作する：[スタッフの操作ガイド](usage.md)
- メニュー・名簿・定型文などを変更する：[やりたいことから探す](howto.md)
- 思いどおりに動かない：[トラブルシューティング](troubleshoot.md)

## 音声について { #audio }

声が小さい・聞こえにくいときの確認手順は、[トラブルシューティング](troubleshoot.md#voice-small)を参照してください。

イヤーマフを使っている人にも、インカムやメガホンの声は聞こえますか？ { #earmuff }
:   聞こえますが、イヤーマフの減衰（外側の音量／Outside Volume）の影響を受けます。0% に設定されていると範囲外の音がすべて遮断されてインカム等の音声も聞こえなくなるため、最低でも 5% 程度確保する運用を推奨します。

イヤーマフを無視して、全員に同じ声の大きさで届ける設定はありますか？
:   ありません。VRChat の仕様上、イヤーマフ処理はワールド側の音声制御よりも後の最終段階で適用されるため、ワールド側からイヤーマフ設定の上書きや状態検知を行うことはできません（[詳細](troubleshoot.md#voice-small)）。

声の大きさを上げれば、イヤーマフで小さくなった分を補えますか？
:   一部しか補えません。[Voice Gain](https://creators.vrchat.com/worlds/udon/players/player-audio/)は VRChat の仕様で上限が 24 dB のため、上げられる幅に限りがあります。

インカムとメガホンの声の大きさは、どこで変えられますか？
:   ワールド全体の既定値はセットアップ窓の「インカム」ページ（1〜24 dB）、スタッフ各自はメニューの[設定タブ](usage.md#voice-gain)にある「声の大きさ」スライダーで調整できます。どちらも「聞く側に届く音量」の設定であり、話す側のマイク音量を変えるものではありません。なお、スタッフ各自のスライダーは自分に聞こえる音量だけを変え、ほかの人の聞こえ方は変わりません（ワールド全体の既定値は、全員の聞こえ方に影響します）。

## ライセンス・購入について

ここは要約です。正式な利用条件は [Staff Bridge System 利用規約（PDF）](https://drive.google.com/file/d/1udZaWP37aN14rFh5DS4WfA0J7ZAQSaax/view?usp=sharing) を参照してください。

複数のワールドで使えますか？
:   購入者本人のワールドであれば使えます。追加購入は不要です。

個人ライセンスとチームライセンスはどう使い分けますか？
:   複数人でのワールド共同開発でもライセンス違反の不安なく使えるよう、人数上限のないチームライセンスを用意しています。
    判定の基準は「何人が編集したか」ではなく、ファイルに何人がアクセスできる状態かです（Git やクラウドストレージでの共有を含みます）。アクセスできる人は全員ライセンスが必要です。

    <div class="license-card-container">
      <div class="license-grid-2">
        <div class="license-box target">
          <h4>制作するとき（対象）</h4>
          <p class="desc">ギミックのファイルに直接アクセスできる人</p>
          <ul>
            <li>ギミック入りのUnityプロジェクトを開く人</li>
            <li>非公開Gitリポジトリに参加している人</li>
            <li>Google Drive / Dropbox 等で共有される人</li>
          </ul>
          <div class="license-tag need">ファイルに触れる人数分が必要</div>
        </div>
        <div class="license-box">
          <h4>公開したあと（対象外）</h4>
          <p class="desc">ワールド内でスタッフ操作・参加する人</p>
          <ul>
            <li>イベントの進行スタッフ</li>
            <li>スタッフ以外の参加者</li>
            <li>ワールドを訪れるすべてのユーザー</li>
          </ul>
          <div class="license-tag free">何人でも購入不要（上限なし）</div>
        </div>
      </div>
      <div class="license-pricing-row">
        <div class="pricing-item">
          <div class="num">触れる人が 1人</div>
          <div class="plan">個人ライセンス × 1</div>
        </div>
        <div class="pricing-item">
          <div class="num">触れる人が 2人</div>
          <div class="plan">個人ライセンス × 2</div>
        </div>
        <div class="pricing-item highlight">
          <div class="num">触れる人が 3人以上</div>
          <div class="plan">★ チームライセンス × 1</div>
        </div>
      </div>
    </div>

    **※ワールドに組み込んだ後、スタッフやスタッフ以外として使うだけの人はカウント対象外です（人数無制限・購入不要）。**

チームライセンスで共有されたアセットは、メンバー個人が自由に持ち出せますか？
:   できません。チームライセンスで共有されたアセットは「そのチームの制作」でのみ使用できます。メンバー個人の所有物にはならないため、個人の別ワールドや他団体で使用する場合は別途ライセンスが必要です。

    <div class="license-rule-list">
      <div class="license-rule-item">
        <div class="license-rule-badge ok">✓</div>
        <div class="license-rule-text">
          <b>同じ運営チームが、別イベントや別ワールドを複数制作する</b>
          <small>→ 1つのチームライセンスで、同一団体が手掛けるすべてのワールドに使用できます。</small>
        </div>
      </div>
      <div class="license-rule-item">
        <div class="license-rule-badge ok">✓</div>
        <div class="license-rule-text">
          <b>プロジェクトの途中で新しい制作メンバーが加入した</b>
          <small>→ 同一団体内の開発者であれば、追加購入することなく共有・作業できます。</small>
        </div>
      </div>
      <div class="license-rule-item">
        <div class="license-rule-badge ng">✕</div>
        <div class="license-rule-text">
          <b>別の運営団体が主催するワールド制作にお手伝いとして参加する</b>
          <small>→ 運営主体が異なるため、その別団体側で新たにライセンスをご用意いただく必要があります。</small>
        </div>
      </div>
      <div class="license-rule-item">
        <div class="license-rule-badge ng">✕</div>
        <div class="license-rule-text">
          <b>共有されたメンバーが、ファイルを私的に持ち出して別ワールドで使う</b>
          <small>→ チームライセンスで共有されたアセットは「そのチームの制作」でのみ使えます。メンバー個人の所有物にはならないため、個人の別ワールドや他団体で使う場合は別途ライセンスが必要です。</small>
        </div>
      </div>
    </div>

チームライセンスは、イベントごとに必要ですか？
:   いいえ。単位はイベントではなく運営団体です。

    <div class="license-rule-list">
      <div class="license-rule-item">
        <div class="license-rule-badge ok">✓</div>
        <div class="license-rule-text">
          <b>同じ運営団体が、定例イベントと周年イベントを別々に開催する</b>
          <small>→ どちらも同一団体の主催であるため、1つのチームライセンスで両方に使えます。</small>
        </div>
      </div>
      <div class="license-rule-item">
        <div class="license-rule-badge ng">✕</div>
        <div class="license-rule-text">
          <b>運営団体Aのスタッフが、別の運営団体Bのイベントにも手伝いで参加する</b>
          <small>→ 運営団体Aのライセンスは運営団体Bでは使えません。運営団体B側で別途ライセンスをご用意ください。</small>
        </div>
      </div>
    </div>

クレジット表記は必要ですか？
:   必須ではありません。記載していただける場合は `© M.G.R` でお願いします。

個人ライセンスとチームライセンスで内容物は違いますか？
:   現行バージョンにおいて、中身や機能の差はありません。主な違いは利用許諾の範囲（共有できる人数）です。

依頼を受けて作るワールドに組み込めますか？（受託制作・コミッション）
:   組み込めます。ただし納品形態によって扱いが異なります。

    <div class="license-rule-list">
      <div class="license-rule-item">
        <div class="license-rule-badge ok">✓</div>
        <div class="license-rule-text">
          <b>組み込み済みのワールドとして納品・アップロード代行する</b>
          <small>→ 制作者側のライセンスのみで可能です（追加購入不要）。</small>
        </div>
      </div>
      <div class="license-rule-item">
        <div class="license-rule-badge ng">✕</div>
        <div class="license-rule-text">
          <b>ギミックのファイル（unitypackageやUnityプロジェクト一式）を依頼主へ引き渡す</b>
          <small>→ 依頼主側でギミックの編集・管理を行う場合は、依頼主側でのライセンス購入が必要です。</small>
        </div>
      </div>
    </div>

購入後の返金はできますか？
:   対応していません。[サンプルワールド](https://vrchat.com/home/world/wrld_01cbbb48-44ce-4761-9baa-6f4ef87fbbfd/info)で動作を確認のうえご購入ください。

アップデートはどう受け取りますか？
:   BOOTH の購入履歴（ライブラリ）から再ダウンロードできます。

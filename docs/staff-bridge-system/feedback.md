# ご意見募集中

Staff Bridge System を触ってのご感想・ご要望をお聞かせください。

<p id="sbs-form-link"></p>
<p id="sbs-form-wait">アンケートは準備中です。もうしばらくお待ちください。</p>

不具合のご連絡や、返信が必要なお問い合わせは
[BOOTH のメッセージ](https://maguro-vrc.booth.pm/) からお願いします。

<script>
// サンプルワールドのゴールボードにはこのページのURLが焼いてある。
// アンケートを差し替えるときは、次の1行だけ直せばよい
// （unitypackage に焼いた文字は後から変えられないので、フォームへ直リンクしない）。
var FORM_URL = "https://forms.gle/3147LFeoz6UBdYat7";

if (FORM_URL) {
  document.getElementById("sbs-form-wait").style.display = "none";
  var a = document.createElement("a");
  a.href = FORM_URL;
  a.textContent = "アンケートを開く";
  document.getElementById("sbs-form-link").appendChild(a);
  location.replace(FORM_URL);   // 自動で移動。戻るボタンでこのページに戻らないよう replace
}
</script>

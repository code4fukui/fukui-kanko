# 福井に関する観光アプリ

1. [ES-Jam](https://code4fukui.github.io/htmlprac/)を開く
2. 下記プログラムを元に作る (参考、[はじめてのJavaScript](https://github.com/code4fukui/slide/blob/main/%E3%81%AF%E3%81%98%E3%82%81%E3%81%A6%E3%81%AEJavaScript.pdf))
```
<script type="module">
import { bg, show } from "https://js.sabae.cc/egadv.js";

await bg();
await show("はろー");
await bg(3972);
let a = await show("ここどこ？", ["福井", "石川", "富山"]);
if (a == "福井") {
  await show("正解！");
}
await show("ぜひ続きを作ってね！");
location = "https://github.com/code4fukui/fukui-kanko/";
</script>
```
3. 自分のGitHubアカウントで新しくリポジトリを作る (アカウントを持っていない方 → [GitHubはじめのいっぽ](https://github.com/code4fukui/slide/blob/main/GitHub%E3%81%AF%E3%81%98%E3%82%81%E3%81%AE%E3%81%84%E3%81%A3%E3%81%BD.pdf))
4. "Add File" → "Create new file"
5. 名前を "index.html" に変更
6. 作ったプログラムを貼り付け
7. 下にスクロールして緑色のボタン "Commit new file" を押す
8. 右上方の "Settings" (隠れている場合は、 ... を押す) → 左メニューの "Pages"
9. "source" を "none" から "main" に変更し、 "Save" を押す
10. 表示されるURLがアプリのURLになる （1分ほど待つと有効になる)
11. このリポジトリの[Issues](https://github.com/code4fukui/fukui-kanko/issues)へぜひご紹介ください！

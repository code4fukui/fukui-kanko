# fukui-kanko

福井県の観光向けに、シンプルでインタラクティブなWebアプリを制作するためのコミュニティプロジェクトです。

このリポジトリは、誰でも簡単にビジュアルノベル形式の小さなWebアプリを構築し、共有できるツールとプラットフォームを提供します。ストーリーを語ったり、クイズを作ったり、福井のお気に入りスポットを案内したりしてみましょう！

## コミュニティ・ショーケース

コミュニティが制作したアプリのギャラリーをご覧ください。ぜひ実際に試して、フィードバックを残したり、インスピレーションを得たりしてください！

➡️ **[Issueでコミュニティのアプリを見る](https://github.com/code4fukui/fukui-kanko/issues)**

## はじめに: オリジナルアプリの作成

以下の手順に従って、オリジナルの福井観光アプリを作成し、公開してみましょう。

### ステップ1: アプリのストーリーを作成する

`index.html` という名前の新しいファイルを作成し、以下のコードを貼り付けます。この例はシンプルなインタラクティブクイズです。Webツール [ES-Jam](https://code4fukui.github.io/htmlprac/) を使えば、ブラウザ上で直接コードをテスト・修正できます。

言語の入門については、[はじめてのJavaScript](https://github.com/code4fukui/slide/blob/main/%E3%81%AF%E3%81%98%E3%82%81%E3%81%A6%E3%81%AEJavaScript.pdf) をご覧ください。

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>My Fukui App</title>
</head>
<body>

<script type="module">
import { bg, show } from "https://js.sabae.cc/egadv.js";

// Set a background image (ID from https://find47.jp/)
await bg(3972); // Tojinbo Cliffs

// Show a message
await show("Hello from Fukui!");

// Ask a question with choices
let answer = await show("Where am I?", ["Fukui", "Ishikawa", "Toyama"]);

// Check the answer and show a result
if (answer == "Fukui") {
  await show("Correct!");
} else {
  await show("Nope, this is in Fukui!");
}

await show("Let's continue exploring!");

// Redirect to the main project page
location.href = "https://github.com/code4fukui/fukui-kanko/";
</script>

</body>
</html>
```

### ステップ2: GitHub Pagesで公開する

1. ご自身のGitHubアカウントで新しいリポジトリを作成します。（GitHubが初めての方は、こちらのガイド [GitHubはじめのいっぽ](https://github.com/code4fukui/slide/blob/main/GitHub%E3%81%AF%E3%81%98%E3%82%81%E3%81%AE%E3%81%84%E3%81%A3%E3%81%BD.pdf) をご参照ください）。
2. 作成した `index.html` ファイルを新しいリポジトリに追加します。
3. リポジトリの **Settings** から **Pages** タブに移動します。
4. 「Build and deployment」の下にあるソースブランチ（例: `main`）を選択し、**Save** をクリックします。
5. GitHubによってサイトが公開され、URL（例: `~~https://your-username.github.io/your-repo-name/`~~ *(unavailable)*）が発行されます。有効になるまで数分かかる場合があります。

### ステップ3: 作成したアプリを共有する

アプリが公開されたら、コミュニティで共有しましょう！

- このリポジトリで **[新しいIssueを作成](https://github.com/code4fukui/fukui-kanko/issues/new)** します。
- アプリのタイトルと、GitHub Pagesで発行されたURLを記載してください。

## サンプルとツール

ご自身のプロジェクトで画像や位置情報を探す際に役立つ、以下のアプリケーションもぜひご活用ください。

- **[キーワード写真検索](https://code4fukui.github.io/find47/search.html)** - キーワードを使って日本全国の風景写真を検索できます。
- **[マップ写真エクスプローラー](https://code4fukui.github.io/find47/map.html)** - 地図を見ながら写真を探すことができます。

## ライセンス

MIT License

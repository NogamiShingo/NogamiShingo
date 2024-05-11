<!---
NogamiShingo/NogamiShingo is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

# 基本的な書き方とフォーマットの構文
[このサイト](https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#headings)を参考に写経。

## 見出し
見出しを作成するには、1つから6つの`#`シンボルを見出しのテキストの前に追加します。使用する`#`の個数によって、見出しの階層レベルと書体のサイズが決まります。
```
# A first-level heading
## A second-level heading
### A third-level heading
```
# A first-level heading
## A second-level heading
### A third-level heading
2つ以上の見出しを使用すると、GitHubでは自動的に目次が生成されます。この目次には、ファイルヘッダー内の三ボタンをクリックするとアクセスできます。各見出しのタイトルが目次に一覧表示され、タイトルをクリックして選択したセクションに移動できます。
![headings-toc](https://github.com/NogamiShingo/NogamiShingo/assets/137843410/5d7a0fa2-424e-419a-9cbf-5c3f35944488)

## テキストのスタイル設定
コメントフィールドと`.md`ファイルでは、太字、斜体、取り消し線、下付き、上付きのテキストで強調を示すことができます。

| スタイル | 構文 | キーボードショートカット | 例 | 出力 |
| :--- | :--- | :--- | :--- | :--- |
| 太字 | `** **`または`__ __` | `ctrl`+`B` | `**This is Bold Text**` | **This is Bold Text**|
| 斜体 | `* *`または`_ _` | `ctrl`+`I` | `_This text is italicized_` | _This text is italicized_|
| 取り消し線 | `~~ ~~` | なし | `~~This was mistaken text~~` | ~~This was mistaken text~~ |
| 太字および太字中にある斜体 | `** **`および`_ _` | なし | `**This text is _extreamely_ important**` | **This text is _extreamely_ important** |
| 全体が太字かつ斜体 | `*** ***` | なし | `***All this text is important***` | ***All this text is important***|
| Subscript | `<sub> </sub>` | なし | `This is a <sub>subscript</sub> text` | This is a <sub>subscript</sub> text|
| Superscript | `<sup> </sup>` | なし | `This is a <sup>superscript</sup> text` | This is a <sup>superscript</sup> text|

## テキストの引用
`>`を使用してテキストを引用符で囲みます。
```
Text that is not a quote

> Text that is a quote
```
Text that is not a quote

> Text that is a quote

引用テキストはインデントされ、種類の異なる色で表示されます。

> [!NOTE]
> 会話を表示するときに、テキストを強調表示して「`R`」と入力することで、コメント内のテキストを自動的に引用符で囲むことができます。・・・をクリックしてコメント全体を引用し、続いて返信を引用します。
> キーボードショートカットについて詳しくは、「[キーボードショートカット](https://docs.github.com/ja/get-started/accessibility/keyboard-shortcuts)」を参照してください。

## コードの引用
単一のバッククォートで文章内のコードやコマンドを引用できます。バッククォート内のテキストはフォーマットされません。また、`ctrl`+`E`キーのキーボードショートカットを押して、Markdown行内にコードブロックのバッククォートを挿入することもできます。
```
Use `Git status` to list all new or modified files that haven't yet been committed.
```
Use `Git status` to list all new or modified files that haven't yet been committed.

独立したブロック内にあるコードあるいはテキストをフォーマットするには、3重のバッククォートを使用します。

````
Some basic Git commands are:
```
git status
git add
git commit
```
````

Some basic Git commands are:
```
git status
git add
git commit
```

詳しくは、「[コードブロックの作成と強調表示](https://docs.github.com/ja/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)」を参照してください。

コードスニペットとテーブルを頻繁に編集する場合は、GitHubのすべてのコメントフィールドで固定幅フォントを有効にするとメリットが得られる可能性があります。詳しくは、「[GitHub上での執筆とフォーマットについて](https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github#enabling-fixed-width-fonts-in-the-editor)」
を参照してください。

## サポートされているカラーモデル
issue、pull request、ディスカッションでは、バックティックを使って文内の色を呼び出すことができます。バックティック内でサポートされているカラーモデルでは、色の視覚化が表示されます。
```
The background color is `#ffffff` for light mode and `#000000` for dark mode.
```
The background color is `#ffffff` for light mode and `#000000` for dark mode.

現在サポートされているカラーモデルを次に示します。

|Color|構文|例|出力|
|:---|:---|:---|:---|
|HEX|``#RRGGBB``|``#0969DA``|`#0969DA`|
|RGB|``rgb(R,G,B)``|``rgb(9,105,218)``|`rgb(9,105,218)`|
|HSL|``hsl(H,S,L)``|``hsl(212,92%,45%)``|`hsl(212,92%,45%)`|

> [!NOTE]
> - サポートされているカラーモデルでは、バックティック内の先頭または末尾にスペースを含めることはできません。
> - 色の視覚化は、issue、pull request、ディスカッション内でのみサポートされます。

## リンク
インラインリンクを作成するには、リンクを角かっこ`[]`で囲み、URLをかっこ`()`で囲みます。
キーボードショートカットの`ctrl`+`K`を使ってリンクを作成することもできます。
テキストを選んだらクリップボードからURLを貼り付け、選択範囲からリンクを自動的に作成できます。

テキストを強調表示し、キーボードショートカット`ctrl`+`V`キーを使うことで、Markdownハイパーリンクを作成することもできます。
テキストをリンクに置き換える場合は、キーボードショートカット`ctrl`+`Shift`+`V`キーを使います。
```
This site was built using [GitHub Pages](https://pages.github.com/).
```
This site was built using [GitHub Pages](https://pages.github.com/).

> [!NOTE]
> GitHubでは、コメント中に適正なURLが記述されていれば自動的にリンクが生成されます。
> 詳しくは、「[自動リンクされた参照とURL](https://docs.github.com/ja/get-started/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls)」を参照してください。

## セクションリンク
セクションの見出しの上にカーソルを移動させてチェーンマークを表示させることにより、表示されたファイル中のセクションに対して直接リンクできます。
![readme-links](https://github.com/NogamiShingo/NogamiShingo/assets/137843410/af1d2400-373a-4d13-9e53-beb03eea3af0)

## Relative links (相対リンク)
表示されたファイル中で相対リンクと画像パスを定義して、読者がリポジトリ中の他のファイルにアクセスしやすくできます。

相対リンクは、現在のファイルに対する相対的なリンクです。
たとえば、リポジトリのルートにREADMEファイルがあり、_docs/CONTRIBUTING.md_ に別のファイルがある場合、READMEの_CONTRIBUTING.md_ への相対リンクは次のようになります。
```
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```
GitHubは相対リンクあるいは画像パスを、現在のブランチに基づいて変換するので、リンクやパスは常にうまく動きます。
リンクのパスは、現在のファイルに対する相対パスになります。`/`で始まるリンクは、リポジトリルートに対する相対パスです。
`./`や`../`のような相対リンクへのオペランドをすべて使用できます。

リンクテキストは1行に記述する必要があります。次の例は機能しません。
```
[Contribution 
guidelines for this project](docs/CONTRIBUTING.md)
```
相対リンクは、リポジトリをクローンするユーザにも扱いやすいです。絶対リンクはリポジトリのクローンではうまく働かないかもしれません。
リポジトリ内の他のファイルを参照するには、相対リンクを使うことをおすすめします。

## 画像
`!`を追加して、代替テキストを`[]`内にラップすると、画像を表示できます。
代替テキストは、画像内の情報に相当する短いテキストです。
次に、画像のリンクをかっこ`()`で囲みます。
```
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)
```
![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

GitHubでは、問題へのイメージの埋め込み、プル要求、ディスカッション、コメントと`.md`ファイルがサポートされます。
リポジトリからイメージを表示したり、オンラインイメージにリンクを追加したり、イメージをアップロードしたりできます。
詳細については、「[アセットをアップロードする](https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#uploading-assets)」を参照してください。

> [!NOTE]
> リポジトリ内の画像を表示する場合は、絶対リンクではなく相対リンクを使います。

相対リンクを使用して画像を表示する例を以下に示します。

|Context|相対リンク|
|:---|:---|
|同じブランチ上の`.md`ファイル内|`/assets/images/electrocat.png`|
|別のブランチ上の`.md`ファイル内|`/../main/assets/images/electrocat.png`|
|リポジトリの問題、プル要求、コメント内|`../blob/main/assets/images/electrocat.png?raw=true`|
|別のリポジトリ内の`.md`ファイル内|`/../../../../github/docs/blob/main/assets/images/electrocat.png`|
|別のリポジトリ内の問題、プル要求、コメント内|`../../../github/docs/blob/main/assets/images/electrocat.png?raw=true`|

> [!NOTE]
> 上の表の最後の二つの相対リンクは、ビューアーがこれらの画像を含むプライベートリポジトリに少なくとも読み取りアクセス権を持っている場合にのみ、プライベートリポジトリの画像に対して機能します。

詳細については、「[相対リンク](https://docs.github.com/ja/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#relative-links)」を参照してください。

### イメージが表示されるテーマの指定
HTMLの`<picture>`要素と`prefers-color-scheme`メディア機能を組み合わせて使って、Markdownで画像が表示されるテーマを指定できます。
淡色モードと濃色モードを区別するため、2つのオプションを使用できます。
これらのオプションを使用して、暗い背景または明るい背景用に最適化された画像を表示できます。
これは、透明なPNGイメージの場合に特に有用です。

たとえば、次のコードでは、明るいテーマの太陽と暗いテーマの月が表示されます。

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>
```
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
  <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
</picture>

URLに追加されたフラグメント(`#gh-dark-mode-only`または`#gh-light-mode-only`)を使うことでテーマに基づいて画像を指定する古い文法は非推奨となり、上記の新しい方法に置き換えられて削除されます。

## リスト
1つまたは複数行の前に`-`、`*`、または`+`を置くことで、順序なしリストを作成できます。
```
- George Washington
* John Adams
+ Thomas Jefferson
```
- George Washington
* John Adams
+ Thomas Jefferson

リストを順序付けするには、名前の前に数字を置きます。
```
1. James Madison
2. James Monroe
3. John Quincy Adams
```
1. James Madison
2. James Monroe
3. John Quincy Adams

### 入れ子になったリスト
1つ以上のリストアイテムをほかのアイテムの下にインデントすることで、入れ子になったリストを作成できます。

GitHub上のWebエディター、または[Vidual Studio Code](https://code.visualstudio.com/)のようなモノスペースフォントを使用するテキストエディターを使って、入れ子になったリストを作成するには、リストが揃って見えるように編集できます。
入れ子になったリスト項目の前に、リストマーカー文字(`-`または`*`)が、その上の項目のテキストの最初の文字の真下に来るまでスペース文字を入力します。 
```
1. First list item
   - First nested list item
     - Second nested list item
```

> [!NOTE]
> Webベースのエディターでは、最初に目的の行を強調表示し、次に`Tab`または`Shift`+`Tab`を使用して、1行以上のテキストをインデントまたはデデントできます。

1. First list item
   - First nested list item
     - Second nested list item

## タスクリスト
タスクリストを作成するには、リストアイテムの前に空白、ハイフン、`[ ]`を付けます。
完了したタスクをマークするには、`[x]`を使います。
```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

タスクリストアイテムの説明がかっこで始まる場合、そのかっこを`\`でエスケープする必要があります。
```
- [ ] \(Optional) Open a followup issue
```
詳しくは、「[タスクリストについて](https://docs.github.com/ja/get-started/writing-on-github/working-with-advanced-formatting/about-task-lists)」を参照してください。

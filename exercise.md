# 演習課題

template/ ディレクトリにある To-do List にはいくつかの問題点があります。それを修正する演習です。

## 作業方法

- 学籍番号のブランチを作成して切り替える
- `submit/` 内に学生番号(小文字)のディレクトリを作成
  - 例: `ht99a999`
- 上記で作成したディレクトリ内に、`template/` の中身をコピー
  - 例
  - ht99a999/
    - index.html
    - main.js
    - ress.css
    - style.css
- [サーバーを起動](#%e3%82%b5%e3%83%bc%e3%83%90%e3%83%bc%e3%81%ae%e8%b5%b7%e5%8b%95%e6%96%b9%e6%b3%95)
- 「[修正内容](#%e4%bf%ae%e6%ad%a3%e5%86%85%e5%ae%b9)」を見て作業

## サーバーの起動方法

開発時には Web サーバーの起動が必要ですが、どんな方法で起動しても構いません。
ここでは、[Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/) を用いたサーバーの起動方法を紹介します。

- Visual Studio Code に `Live Server` という拡張機能を導入
  - Visual Studio Code の左側から拡張機能のタブを開いて検索

![install Live Server](https://i.imgur.com/gRO7bug.png)

- html ファイルが入っているディレクトリを Visual Studio Code で開く
  - ドラッグ & ドロップで開けます
- 右下の `Go Live` をクリックしてサーバーを起動
  - 起動時にポート番号が競合してなければ <http://localhost:5500/> でアクセス可能
  - 停止するには右下の `Port : xxxx` と書いてるところを選択

![server run](https://i.imgur.com/4sEmRsk.png)

## 修正内容

### [Delete selected items] ボタンから、選択された項目を削除する関数 deleteSelected() を呼び出すように

コピー直後のサイトにアクセスし、テキストボックスに適当な値を入力し [Add to-do] を押してデータを追加します。
追加されたら、項目の左側にチェックを入れて [Delete selected items] を押してみましょう。
現時点では削除されないことが確認できると思います。
これは、 deleteSelected() が呼び出されていないので、index.html にあるボタンから呼び出す処理を追加してコミットしましょう。

- 処理を追加した後は以下のようになります。

![delete-selected](https://i.imgur.com/rYK0iAC.gif)

### 大見出しを中央揃えに

大見出し (h1) が左側に寄っているので、 style.css で中央揃えに設定してコミットしましょう。

- 大見出しを中央揃えにしたら以下のような画面になります。

![centering](https://i.imgur.com/prNsBov.png)

### body に対して Google Fonts を導入

Google Fonts から、好きな日本語フォントを導入してコミットしましょう。

- Google Fonts を導入したら以下のような画面になります。（完成）

![Google Fonts](https://i.imgur.com/FiBKY5t.png)

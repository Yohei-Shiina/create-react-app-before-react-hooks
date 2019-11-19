# create-react-app-output-before-react-hooks
## 学習用の古いバージョンのReact

udemyやその他動画等でreactの学習をローカル環境で始めるため、

`create-react-app` を実行する

その後サーバーを立ち上げて確認。

すると、udemyやその他動画等と自分ので作ったファイルの内容やフォルダ構成等が一致しない場合がある。

- reactのロゴがくるくるしてるやつと

- くるくるしていない動きのない本みたいなやつ

ファイルの内容も以下のように違う。

create-react-app コマンドでできた雛形の App.jsに２パターン

```
function App() {
..
```

```
Class App Extends Component {
・・
```
create-react-appのバージョン違いによるものらしい

## その経緯

現在は function App()という上記の書き方が主流

こちらに変わったのはReact Hooksを使うようになったからぽい

[参照テラテイル記事](https://teratail.com/questions/219832)

ただ学習したいだけだから、よく使われてる古いバージョンのやつクローンできたらいいよねってことでこのリポジトリを準備した

# TODO

まずはクローン
 
`git clone https://github.com/Yohei-Shiina/create-react-app-before-react-hooks.git `

登録されているremoteのリポジトリをremove

`git remote rm origin`

githubでリポジトリを新規作成

新規作成したリポジトリのURLを取得してそのURLをリモート先として登録

`$ git remote add origin ここにgithubで作ったリポジトリのURL`  
  
リモートにプッシュ（ 'master' のみだとエラー吐くので '+' をつける）  
  
`git push origin +master`  
  
できたら準備OK　開発するのみ

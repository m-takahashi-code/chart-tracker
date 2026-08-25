# 新店チャート手配台帳

カラーチャート／ストーンチャート／サンプルオプションの新店舗向け作成・在庫振り分け状況を管理するツールです。

## GitHubで公開する手順（GitHub Pages）

1. GitHubで新しいリポジトリを作成する（例：`chart-tracker`）
   - Public / Private どちらでも可（Pagesを使うだけならPublic推奨）
2. このフォルダ内の `index.html` をリポジトリのルートにアップロードする
   - GitHubの画面右上「Add file」→「Upload files」からドラッグ＆ドロップでOK
3. リポジトリの **Settings → Pages** を開く
4. 「Build and deployment」の Source を **Deploy from a branch** にし、Branch を `main` / `/(root)` に設定して保存
5. 数分後、`https://ユーザー名.github.io/リポジトリ名/` でアクセスできるようになります

## 注意点（重要）

- データ保存には **ブラウザのlocalStorage** を使用しています
  - 同じブラウザ・同じ端末でアクセスした場合のみ、入力内容が保持されます
  - 別の端末やブラウザ、シークレットモードでは保存内容が共有されません
  - 複数人でリアルタイムに共有したい場合は、別途データベース（Firebase等）との連携が必要です
- ブラウザのキャッシュ削除・localStorage消去を行うとデータが消えます。定期的に大事な内容はメモ等に控えることをおすすめします

## ローカルで試す

`index.html` をそのままダブルクリックしてブラウザで開くだけで動作します。

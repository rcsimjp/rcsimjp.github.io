# RoboCup SimJP

https://rcsimjp.github.io/

ロボカップシミュレーションリーグ 日本コミュニティのWebサイト（予定）です．

## サイト更新手順

各ページのソースとなるMarkDownファイルをmasterブランチへpushすることで、自動的にWebページが生成されます。
ページのデプロイにはpushから少し時間がかかることがあります。

ローカルで動作確認するには、自分の環境に[Jekyllを設定](https://jekyllrb.com/docs/installation/)する必要があります。
詳細は[GitHub Pagesのドキュメント](https://docs.github.com/ja/pages)を参照してください．

1. mdファイルを更新する
2. bundle installを実行
```
bundle install
```
3. ローカルでJekyllサイトを実行
```
bundle exec jekyll serve
```
4. Webブラウザで `http://localhost:4000` を開いて確認。
ローカルサイト実行中にmdファイルを更新すると、裏でhtmlファイルも更新されている。
mdファイルの編集結果の確認だけなら、ブラウザをリロードするだけで良い。

### ブログ形式の投稿

_post以下に `日付-タイトル.md` (`YYYY-MM-DD-Title.md`) という名前でファイルを追加すると、自動的にその日付の投稿となります。
内部のヘッダ部分で表示するタイトル、投稿日時、カテゴリなどを指定できます。

投稿のRSSフィードも自動生成されるので、お知らせに利用すると良いでしょう。





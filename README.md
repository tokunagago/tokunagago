# tokunagago.github.io


Hugoトップディレクトリ
~/go-blog

Hugoトップディレクトリ/config.toml で基本設定
```
baseURL = 'https://[GitHubユーザ名].github.io/'
languageCode = 'ja-jp'
title = '任意のブログタイトル'
theme = '適用するテーマ名'
```

記事の作成
`hugo new post/タイトル名.md`
Hugoトップディレクトリ/content/post/`タイトル名`.mdが生成される

ローカルでチェック
`hugo server`

公開用リソースを作成。publicディレクトリが生成される。
`hugo -D`

生成されたpulicディレクトリの中身をGithub pagesにコピー
`cp -pr /path/to/Hugoトップディレクトリ/public/* /path/to/[ユーザ名].github.io/`
（`cp -pr /Users/tokunagago/go-blog/public/* /Users/tokunagago/tokunagago`）

Githubに変更を反映
```
cd [ユーザ名].github.io/
git add .
git commit -m "Initial commit"
git push -u origin master
```

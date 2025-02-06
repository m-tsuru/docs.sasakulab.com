+++
title = 'Hugo でテーマからスクラッチする'
date = 2025-02-06T16:00:00+09:00
draft = false
summary = 'docs.sasakulab.com を形成する Hugo について，その過程を残しています'
categories = ["Go"]
tags = ["Go", "Hugo", "乱文"]
+++

`docs.sasakulab.com` は Hugo で作られています．

## インストール

```sh
brew install hugo
```

## サイト作成

```sh
hugo new site site-name
cd site-name
git init
hugo server
```

`hugo server` で [http://localhost:1313](http://localhost:1313) ホストされる．

正常に (Page Not Found と言われるから異常に？) ホストされたら準備完了．`^C`で抜ける．

## テーマ作成

```sh
hugo new theme theme-name
```

すると，`themes/theme-name` に新しいテーマができる．

これを編集することで，最終的に完成する．頑張ってください．

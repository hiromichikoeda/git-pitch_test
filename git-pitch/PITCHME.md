# Git Pitch

---
### スライド作成手順はこれだけ

1. Githubでリポジトリを用意
1. PITCHME.mdを作成
1. markdown記法で記述する
1. 変更をpuh!


---
このようなURLにアクセス出来るようになっているはずです

- リポジトリ直下にPITCHME.mdを置いた場合

`https://gitpitch.com/[ユーザー名]/[リポジトリ名]`

- サブディレクトリで管理する場合

`https://gitpitch.com/[ユーザー名]/[リポジトリ名]?p=[サブディレクトリ名]`

- 例：このスライド自身のURL

https://gitpitch.com/hiromichikoeda/techshare?p=git-pitch


---
### 「Git Pitch」を使うメリット・デメリット
- 😁 Githubアカウントがあればすぐ外部公開用URL付きのスライドが簡単に作成できる|
- 😁 markdownで書けるので簡単|
- 😁 Github上で管理・編集できるのでローカルでファイルを管理しなくて良い。（もちろんローカルのcloneしてきて編集することも可能）|
- 😵 プライベートリポジトリは現在サポートされていないので閲覧者を制限したいという用途では使えない|


---
### 基本的な書き方

####`---`でページを区切る

```md
---
###ページ１
これは１ページ目
---
###ページ２
これは２ページ目
```

---?code=sample.js
`---?code=sample.js`の様に記述するとリポジトリ内ファイルを表示できる（リポジトリ内のsample.jsを表示中）


---?include=［ディレクトリ]/[ファイル名]
`---?include=［ディレクトリ]/[ファイル名]`を記述で外部のmdファイルをインクルード出来る（自己紹介ページとか分けておくと便利かも）
 
?p=で繋げばディレクトりも分けて管理できる
https://gitpitch.com/[ユーザー名]/[リポジトリ名]?p=[サブディレクトリ名]


---
### 実際に作ったスライド
  https://gitpitch.com/hiromichikoeda/techshare/
  https://gitpitch.com/hiromichikoeda/techshare?p=sample
  https://gitpitch.com/hiromichikoeda/techshare?p=git-pitch

---
### 運用上の問題点

### おわり

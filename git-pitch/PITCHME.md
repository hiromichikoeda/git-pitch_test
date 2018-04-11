
### 「Git Pitch」で公開用スライドを作成する

---
### スライド作成手順はこれだけ

- Githubでリポジトリを用意
- PITCHME.mdを作成
- markdown記法で記述する
- 変更をpuh!


---
####このようなURLにアクセス出来るようになっているはずです。(リポジトリ直下にPITCHME.mdを置いた場合は【?p=[サブディレクトリ名]】は不要)

`https://gitpitch.com/[ユーザー名]/[リポジトリ名]`
`https://gitpitch.com/[ユーザー名]/[リポジトリ名]?p=[サブディレクトリ名]`

このスライド自身のURL

https://gitpitch.com/hiromichikoeda/techshare?p=git-pitch


---
### 「Git Pitch」を使うメリット・デメリット
####メリット
- Githubアカウントがあればすぐ外部公開用URL付きのスライドが簡単に作成できる|
 * プライベートリポジトリは現在サポートされていないので閲覧者を制限したいという用途では使えない||
- markdownで書けるので簡単|
- Github上で管理・編集できるのでローカルでファイルを管理しなくて良い。（もちろんローカルのcloneしてきて編集することも可能）|




---
### 基本的な書き方

- `---`でページを区切る

```md
---
###ページ１
これは１ページ目
---
###ページ２
これは２ページ目
```

---?code=sample.js
外部コードの読み込み


---?include=［ディレクトリ]/[ファイル名]
をPITCHME.mdに記述で外部のmdファイルをインクルード出来る（自己紹介ページとか分けておくと便利かも）
 
?p=で繋げばディレクトりも分けて管理できる
https://gitpitch.com/[ユーザー名]/[リポジトリ名]?p=[サブディレクトリ名]


---
### 実際に作ったスライド
  https://gitpitch.com/hiromichikoeda/techshare/
  https://gitpitch.com/hiromichikoeda/techshare?p=sample
  https://gitpitch.com/hiromichikoeda/techshare?p=git-pitch

---


### おわり

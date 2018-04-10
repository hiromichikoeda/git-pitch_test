
### 「Git Pitch」の使い方:octocat:

---
### スライド作成手順

- 既存でも新規でもよいのでリポジトリを用意
- PITCHME.mdを作成|
- markdown記法で記述する(`---`でスライドのページを区切る)|
- 変更をpuh!|


---
### スライド作成手順
- `https://gitpitch.com/[ユーザー名]/[リポジトリ名]?p=[サブディレクトリ名]`
- ↑このようなURLにアクセス出来るようになっているはずです。(リポジトリ直下にPITCHME.mdを置いた場合は【?p=[サブディレクトリ名]】は不要)


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

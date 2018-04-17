# 「Netlify CMS」
で管理画面を作る


---
## さっそくデモ
https://techlife-koe.netlify.com/admin/


---
## やり方
1. Githubでアプリケーションを登録
1. NetlifyをGithubを連携
1. 記事を保存しているディレクトリに '/admin' を作成
1. admin内に「index.html」と「config.yml」を作成し各種設定を記述


---
### Githubでアプリケーションを登録する
<img src="https://github.com/hiromichikoeda/techshare/netlify-cms/assets/images/2018-04-12 13.52.56.png">
[Developer applications](https://github.com/settings/developers)からアプリケーションを登録します。

![アプリケーション登録](netlify-cms/assets/images/2018-04-12 13.52.56.png)
Authorization callback URLには 'https://api.netlify.com/auth/done' を指定します。
それ以外は自由に記載してOKです。






---
## 参考
[Netlify公式ブログ](https://www.netlify.com/blog/2015/10/26/a-step-by-step-guide-hexo-on-netlify/)の手順通り進めるとわかりやすいです。


---
### Netlify CMS

Netlify が提供している CMS

---

### 手順
[Githubのdevelopers](https://github.com/settings/developers)の「New OAuth App」からアプリケーションを登録する


- 「Authorization callback URL」には「https://api.netlify.com/auth/done」と入力し、それ以外は適宜入力で大丈夫です

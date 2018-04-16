# 「Netlify CMS」で管理画面を作る

---
## さっそくデモ
https://techlife-koe.netlify.com


---
## さっそくデモ
https://techlife-koe.netlify.com/admin

netlifyで作成したサイトのURLに/adminを付ける


---
[Netlify公式ブログ](https://www.netlify.com/blog/2015/10/26/a-step-by-step-guide-hexo-on-netlify/)の手順通り進めるとわかりやすいです。


---
### Netlify CMS

Netlify が提供している CMS

---

### 手順
[Githubのdevelopers](https://github.com/settings/developers)の「New OAuth App」からアプリケーションを登録する

<img src="https://github.com/hiromichikoeda/techshare/blob/master/netlify-cms/images/2018-04-12%2013.52.56.png">


- 「Authorization callback URL」には「https://api.netlify.com/auth/done」と入力し、それ以外は適宜入力で大丈夫です

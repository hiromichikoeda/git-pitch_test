# 「Netlify CMS」
で管理画面を作る

---
## 「Netlify」
静的コンテンツをベースにしたWebサイトのホスティングに特化したサービス。「Hexo」や「Hugo」などの静的サイトジェネレータでWebサイトを作って公開できる。

[Netlify公式ブログ](https://www.netlify.com/blog/2015/10/26/a-step-by-step-guide-hexo-on-netlify/)の手順通り進めるとわかりやすいです。


---
## 「Netlify CMS」
Netlifyをwordpressのように管理画面で管理することができる


---
## 管理画面DEMO
https://techlife-koe.netlify.com/admin/


---
## やり方
1. [Github](https://github.com/settings/developers)からアプリケーションを登録（Client IDとClient Secretは後で必要なので控えてください）
1. [NetlifyのOAuth認証の登録画面](https://app.netlify.com/sites/techlife-koe/settings/access)でアプリを連携
1. 記事を保存しているディレクトリに '/admin' を作成
1. admin内に「index.html」と「config.yml」を作成し各種設定を記述

---
'''

'''

---
'''
'''
---
config.ymlは以下参照。

[Netlify CMS公式 |Configuration Options](https://www.netlifycms.org/docs/configuration-options/)

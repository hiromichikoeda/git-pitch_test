# 「Netlify CMS」
で管理画面を作る

---
## 「Netlify」
静的コンテンツをベースにしたWebサイトのホスティングに特化したサービスで、「Hexo」や「Hugo」などの静的サイトジェネレータでWebサイトを作って公開できます。

[参考 | Netlify公式ブログ](https://www.netlify.com/blog/2015/10/26/a-step-by-step-guide-hexo-on-netlify/)がわかりやすいです。


---
## 「Netlify CMS」
NetlifyをWordPressのように管理画面で管理することができます。


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
index.html
```.html
<!doctype html>
<html>
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Content Manager</title>

  <link rel="stylesheet" href="https://unpkg.com/netlify-cms@^0.3/dist/cms.css" />

</head>
<body>
  <script src="https://unpkg.com/netlify-cms@^0.3/dist/cms.js"></script>
  <script>
    CMS.registerPreviewStyle('/css/main.css');
  </script>
</body>
</html>
```

[参考 | Netlify CMS公式 | App File Structure](https://www.netlifycms.org/docs/add-to-your-site/#app-file-structure)

---
config.yml
```.yml
backend:
  name: github
  repo: hiromichikoeda/hexo-netlify
  branch: master

publish_mode: editorial_workflow

media_folder: "static/images/uploads"
public_folder: "source/images/uploads"

collections:
- name: "blog" # Used in routes, e.g. /admin/collections/blog
  label: "Blog" # Used in the UI
  folder: "source/_posts" # The path to the folder where the documents are stored
  create: true # Allow users to create new documents in this collection
  slug: "{{slug}}"
  fields:
    - {label: "Title", name: "title", widget: "string"}
    - {label: "Publish Date", name: "date", widget: "datetime", default: ""}
    - {label: "Categories", name: "categories", widget: "list", default: ""}
    - {label: "Image", name: "image", widget: "image", required: false}
    - {label: "Content", name: "body", widget: "markdown"}
    - {label: "Layout", name: "layout", widget: "hidden", default: "blog"}
  meta:
    - {label: "Tags", name: "tags", widget: "list", default: "" }, default: "" }

```

[参考 | Netlify CMS公式 | Configuration Options](https://www.netlifycms.org/docs/configuration-options/)

---
設定を駆使するとこんな画面がつくれそう。

[Netlify公式demo]（https://cms-demo.netlify.com/#/collections/posts)

---
### 使用した感想
- Git分からない人でも簡単に記事をアップできる
- 設定画面を作り込むのが面倒そう
- 慣れているならエディタ上で編集してcommitのほうが早そう

---
おしまい😉

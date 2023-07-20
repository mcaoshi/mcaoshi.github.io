# 设置

自定义您的网站主题颜色、布局、标题等。设置文件存放在 `src/yml`目录下.

## 网站

常规设置储存在 [`src/yml/site.yml`](https://github.com/thiagorossener/jekflix-template/blob/master/src/yml/site.yml)目录下.

> **重要提示：** 仅在克隆存储库时。如果您使用的是 `gem`, 修改这些属性 `_config.yml`。

#### `name`

类型：*字符串*

网站名称将出现在几个地方，最重要的一个在标题处。

例如：

```yaml
# site.yml
name: Jekflix
```

#### `标题e`

类型：*字符串*

网站标题用于SEO目的并设置主页标题。

例如：

```yaml
# site.yml
title: Jekflix | A blog theme for Jekyll
```

#### `描述`网站标签用作SEO目的的关键字。

Type: *string*

网站描述仅用于SEO目的.

例如：

```yaml
# site.yml
description: Jekflix is a template for Jekyll inspired by Netflix and made by Thiago Rossener.
```

#### `标签`

Type: *list*

网站标签用作SEO目的的关键字.

例如：

```yaml
# site.yml
tags:
  - blog
  - template
  - jekyll
  - theme
  - netlify
```

#### `email`

类型：*字符串*

该电子邮件用于带有旧版 [Formspree](https://formspree.io/) 表单的“联系人”页面。

将此和`formspree_form_id`留空不会显示“联系人”页面。

> **警告：** 这将在 v4 中过时


例如：

```yaml
# site.yml
email: youremail@xyz.com
```

#### `表单预置表单 ID `

类型：*字符串*

[表单](https://formspree.io/) ID 在联系人页面中使用。

将此内容和“电子邮件”留空不会显示“联系人”页面。

例如：


```yaml
# site.yml
formspree_form_id: your_formspree_form_id
```

#### `disqus_username`

类型：*字符串*

设置您的 [Disqus](https://disqus.com)用户名以在您的帖子中添加评论。如果您不想启用注释，请将其留空。

例如：

```yaml
# site.yml
disqus_username: disqus_username
```

#### `首页大图`

类型：*布尔值*

在主页中 显示/隐藏它,它接受值`true` 和 `false`。

例如：

```yaml
# site.yml
show_hero: true
```

![Home page with hero screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566477681/page-with-hero-screenshot_ixyjzp.jpg)

>没有首页大图的例子

```yaml
# site.yml
show_hero: false
```

![Home page without hero screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566477862/page-without-hero-screenshot_gobnva.jpg)

#### `标页数`

类型：*整数*

将分页添加到主页。

将一个整数设置为 0 >，表示每页要显示的帖子数,如果您不想分页，请将其留空。

```yaml
# site.yml
paginate: 12
```

## Social

社交设置可以在 [`src/yml/social.yml`](https://github.com/thiagorossener/jekflix-template/blob/master/src/yml/social.yml). 社交媒体图标出现在每个页面的页脚中。

> **重要：** 仅在克隆存储库时。如果您使用的是“gem”，请在`_config.yml`。

#### `github_username`

类型：*字符串*

设置网站的 GitHub 用户名。

```yaml
# social.yml
github_username: github_username
```

#### `facebook_username`

类型：*字符串*

为网站设置脸书用户名。

```yaml
# social.yml
facebook_username: facebook_username
```

#### `twitter_username`

类型：*字符串*

设置网站的推特用户名。

```yaml
# social.yml
twitter_username: twitter_username
```

#### `instagram_username`

类型：*字符串*

设置网站的Instagram用户名。

```yaml
# social.yml
instagram_username: instagram_username
```

#### `linkedin_username`

类型：*字符串*

设置网站的LinkedIn用户名。

```yaml
# social.yml
linkedin_username: linkedin_username
```

#### `medium_username`

类型：*字符串*

设置网站的Medium username用户名。

```yaml
# social.yml
medium_username: medium_username
```

## 主题

主题设置在 [`src/yml/theme.yml`](https://github.com/thiagorossener/jekflix-template/blob/master/src/yml/theme.yml). 您只需要更改此文件并运行 `gulp build`。

> **重要提示：** 仅在克隆存储库时。如果您使用的是“宝石”，请按照以下操作 [these instructions](https://github.com/thiagorossener/jekflix-template#theme-colors).

### GitHub pages

这是一个已知问题，即在将网站部署到 GitHub 页面时无法运行 Gulp。因此，您必须更改主题颜色并在本地运行`gulp build` ，然后将更改推送到您的存储库中，没有其他方法。

要查看部署网站时的外观，请运行`bundle exec jekyll serve` 和访问 `http://127.0.0.1:4000/`.

#### `主题颜色`

类型：*十六进制*

Default: ![#ff0a16](https://placehold.it/15/ff0a16/000000?text=+) `#FF0A16`

链接、图标和一些自定义元素中使用的颜色。

```yaml
# theme.yml
themeColor: "#ff0a16"
```

#### `primaryDark`

类型：*十六进制*

Default: ![#141414](https://placehold.it/15/141414/000000?text=+) `#141414`

深色背景和某些文本中使用的颜色。

```yaml
# theme.yml
primaryDark: "#141414"
```

#### `深色`

类型：*十六进制*

Default: ![#ffffff](https://placehold.it/15/ffffff/000000?text=+) `#FFFFFF`

用于浅色背景和与深色背景对比的颜色.

```yaml
# theme.yml
accentDark: "#ffffff"
```

#### `浅色`

类型：*十六进制*

Default: ![#f2f2f2](https://placehold.it/15/f2f2f2/000000?text=+) `#F2F2F2`

边框中使用的颜色，与浅色背景的对比，一些链接和字幕.

```yaml
# theme.yml
lightGray: "#f2f2f2"
```

#### `文本`

类型：*十六进制*

Default: ![#333333](https://placehold.it/15/333333/000000?text=+) `#333333`

整体文本中使用的颜色.

```yaml
# theme.yml
texts: "#333333"
```

## Posts

帖子设置可以在 [`src/yml/posts.yml`](https://github.com/thiagorossener/jekflix-template/blob/master/src/yml/posts.yml).

> **重要提示：** 仅在克隆存储库时。如果您使用的是`gem`，请在 `_config.yml`.

#### `显示时间栏`

类型：*布尔值*

显示/隐藏阅读进度条。它接受值 `true` 或 `false`.

```yaml
# posts.yml
show_time_bar: true
```

![阅读进度条截图](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566425470/progress-bar-screenshot_gem7xb.jpg)

#### `退出时显示模态`

类型：*布尔值*

当访问者离开页面时显示/隐藏推荐模式。它接受值 `true` 和 `false`.

```yaml
# posts.yml
show_modal_on_exit: false
```

![模态截图](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566478245/before-you-go-screenshot_prrplk.jpg)

#### `到达页面终点时的显示模态`

类型：*布尔值*

当访问者到达帖子末尾时显示/隐藏推荐模式。它接受值 `true` or `false`.

```yaml
# posts.yml
show_modal_on_finish_post: false
```

![Modal screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566478245/before-you-go-screenshot_prrplk.jpg)

#### `two_columns_layout`

类型：*布尔值*

在一列和两列之间切换帖子布局。它接受值`true` or `false`.

>两列示例：

```yaml
# posts.yml
two_columns_layout: true
```

![带有两列帖子的样式](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566476793/two-columns-screenshot_phumrl.jpg)

>一列示例：

```yaml
# posts.yml
two_columns_layout: false
```

![带有一列帖子的样式](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566476792/one-column-screenshot_m1k0xt.jpg)

## 高深

高级设置可以在 [`src/yml/advanced.yml`](https://github.com/thiagorossener/jekflix-template/blob/master/src/yml/advanced.yml).

>**重要提示：** 仅在克隆存储库时。如果您使用的是`gem`，请在 `_config.yml`.

#### `baseurl`

类型：*字符串*

设置网站的子路径，例如 `/blog`.

```yaml
# advanced.yml
baseurl: ""
```

#### `url`

类型：*字符串*

为您的网站设置基本主机名和协议，例如 `https://rossener.com`

```yaml
# advanced.yml
url: ""
```

#### `谷歌分析`

类型：*字符串*

设置您的谷歌分析 [tracking ID](https://www.youtube.com/watch?v=Mtzl4tkVdbI).

```yaml
# advanced.yml
google_analytics: "UA-XXXXXXXX-X"
```

#### `语言`

类型：*字符串*

设置您的网站语言。它用于SEO目的（例如 `pt-BR`, `en`, `es`, `fr`)

```yaml
# advanced.yml
language: "en"
```

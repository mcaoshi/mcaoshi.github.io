# Post

## 创建帖子

克隆repo时，可以使用`initpost.sh`脚本生成新的post（该脚本在`gem`中不可用）。

要执行此操作，只需在项目目录中运行：

```
./initpost.sh -c "Your Post Title"
```

新文件将在`_posts'目录中创建，格式为`YYYY-MM-DD-标题.md`。

## Front Matter属性

>如果您不知道这些是什么，请检查 Jekyll 的 [文档](https://jekyllrb.com/docs/front-matter/)。

*Jekflix* 发布post文件如下所示：

```yaml
# _posts/2010-01-01-标题.md

---
date: 2019-05-16 23:48:05
layout: post
title: 标题
subtitle: 副标题
description: 描述.
image: 图片
optimized_image: 优化的图片
category: 分类
tags:
  - 标签1
  - 标签2
  - 标签3 
author: 发布的作者
paginate: true
---
```

以下是模板的完整列表  Matter properties 解释:

#### `日期`

类型： *日期时间*

发布后日期。格式： `YYYY-MM-DD hh:mm:ss`

例如：

```yaml
# _posts/2022-08-22-example.md
---

date: 2022-05-16 23:48:05

---
```

#### `布局`

类型：*字符串*

>将使用的布局文件。该模板只有一个有效的帖子布局，即 `post`.

```yaml
# _posts/2022-08-22-example.md
---

layout: post

---
```

#### `标题`

类型：*字符串*

>帖子的标题。

例如：

```yaml
# _posts/2022-08-22-example.md
---

title: 小明回家就会被揍，为什么

---
```

#### `副标题`

*（可选）*

类型：*字符串*

>帖子副标题。它显示在标题下方。

例如：

```yaml
# _posts/2022-08-22-example.md
---

subtitle: 可能是因为在学校调皮被老师请家长

---
```

#### `描述`

类型：*字符串*

>帖子描述。它用于主页和类别页面，用于SEO目的和社交媒体共享的元描述标签。

例如：

```yaml
# _posts/2022-08-22-example.md
---

description: 这次请家长可能最重要的原因是，小明把女同学的衣服撕破了。

---
```

#### `图片`

类型：*url*

>特色图片。它用于主页和类别页面以及社交媒体共享，可以使图片超链接和本地上传。

**提示：** 使用媒体服务器为您的网站提供图像，例如 [Cloudinary](https://cloudinary.com)

*Obs：推荐的图像分辨率为 760x399*

例如：

```yaml
# _posts/2022-08-22-example.md
---

image: https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559821647/theme6_qeeojf.jpg

---
```

#### `优化的图像`

*（可选*）

类型：*url*

>优化的特色图片。设置较小的图像以显示在主页和类别页面中，它们将加载得更快。
如果没有设置“optimized_image”，页面将显示“image”中的图片。

*Obs：建议的图像分辨率为 380x200*

例如：

```yaml
# _posts/2019-08-22-example.md
---

optimized_image: https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559821647/theme6_qeeojf.jpg

---
```

#### `类别`

类型：*字符串*

>只允许一个类别。如果是<category>.md，请确保在“类别”目录中创建一个“.md”文件。

例如：

```yaml
# _posts/2022-08-22-example.md
---

category: 水果

---
```

#### “标签”

类型： *列表*

>帖子关键字列表。它用于主页，类别和标签页面，并用作SEO目的的元关键字。

例如：

```yaml
# _posts/2022-08-22-example.md
---

tags:
  - 葡萄
  - 桃子

---
```

#### “作者”

*（可选）*

类型：*字符串*

>帖子作者。设置`_authors`文件夹中使用的作者文件名。
每次创建新作者时，请确保在其中也创建一个文件。
如果没有作者，请将其留空。

例如：

```yaml
# _posts/2019-08-22-example.md
---

author: 樱桃酱

---
```

#### `标页数`

*（可选）*

类型：*布尔值*

>要将帖子分成几页，请将属性`paginate`设置为`true` ，并在要中断的位置使用分隔符 `--page-break--` 

**注意：** 该模板使用`jekyll-paginate-content`，[GitHub 页面不支持](https://pages.github.com/versions/)。如果您需要该功能，请部署到其他位置。

例如：

```yaml
# 2022-08-20-ten-skills-you-need-to-have-to-become-a-good-developer.md
---

paginate: true

---

Skill 1

--page-break--

Skill 2
```

如下图:

![Paginated Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566430021/paginated-page-screenshot_zx4xjn.jpg)

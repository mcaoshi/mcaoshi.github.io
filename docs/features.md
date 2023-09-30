# Features

_Jekflix_ 具有帮助您创建/编辑/共享内容并为访问者提供良好体验的功能.

- [在线搜索](docs/features.md#live-search)
- [预设阅读时间](docs/features.md#estimated-reading-time)
- [阅读进度条（可选）](docs/features.md#reading-progress-bar) 
- [新帖子 标签](docs/features.md#new-post-tag)
- [按需加载图像](docs/features.md#load-images-on-demand)
- [推送菜单](docs/features.md#push-menu)
- [SVG 图标](docs/features.md#svg-icons)
- [用于创建帖子的脚本](docs/features.md#shell-script-to-create-posts)
- [标签页面](docs/features.md#tags-page)
- [关于页面](docs/features.md#about-page)
- [联系页面](docs/features.md#contact-page)
- [404 错误页](docs/features.md#404-error-page)
- [提要 RSS](docs/features.md#feed-rss)
- [Disqus（可选）](docs/features.md#disqus) 
- [精选帖子（可选）](docs/features.md#featured-post) 
- [主页分页（可选）](docs/features.md#home-page-pagination)
- [帖子侧边栏（可选）](docs/features.md#posts-sidebar)
- [分页帖子（可选）](docs/features.md#paginated-posts) 
- [触发模式（可选）](docs/features.md#before-you-go-modal) 
- [帖子推荐](docs/features.md#post-recommendation)
- [Netlify CMS](docs/features.md#netlify-cms-ready)
- [翻译新！](docs/setup.md#translations) **new!**
- [数学表达式（可选）新增！](docs/features.md#math-expressions) **new!**

## 在线搜索

搜索组件位于模板的右上角，用于查找帖子标题、类别和标签。这是对静态网站的简单搜索。

![Search Box Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566426001/search-screenshot_sc5edu.jpg)

## 预计阅读时间

每个帖子在其标题上方显示估计的阅读时间，分钟是根据平均读者速度计算的。

![Estimated Reading Time Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566426097/minutes-to-read-screenshot_akvu69.jpg)

## 阅读进度条

*(Optional)*

它还根据阅读时间和页面中的滚动位置显示阅读进度条.

![Reading Progress Bar Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566425470/progress-bar-screenshot_gem7xb.jpg)

您可以显示/隐藏时间栏，请参阅 [docs](settings.md#show_time_bar).

## "New Post" tag

对于在当前日期前 7 天内发布的帖子，系统会在主页中附加一个“新帖子”标签.

![New Post Tag Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566425920/new-post-tag-screenshot_nyuycr.jpg)

## 按需加载图像

为了提高主页的性能，最初仅加载首屏以上的帖子。根据需要向下滚动时加载下一篇文章.

![Loading Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566426573/loading-screenshot_akchmx.jpg)

## 推送菜单

模板菜单默认隐藏，打开时将内容向右推送.

![Menu Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566426941/menu-screenshot_qsoz1z.jpg)

## SVG 图标

模板中使用的所有图标都是 SVG，为每种分辨率提供漂亮的外观.

![Template Icons](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566427250/icons-screenshot_uhk80e.jpg)

## 用于创建帖子的外壳脚本

名为 [initpost.sh](https://github.com/thiagorossener/jekflix-template/blob/master/initpost.sh) 提供是为了更容易通过命令行创建帖子.

在项目目录中，只需运行:

```
$ ./initpost.sh -c "New post title"
```

## 标签页面

所有标签都收集在一个页面中，访问者可以在其中找到由其标签分隔的博客文章。

![Tags Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566430436/tags-page-screenshot_eeyyt8.jpg)

Check it out [here](https://jekflix.rossener.com/tags/).

## About page

默认情况下提供关于页面，您可以随时将其删除.

![About Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566430703/about-page-screenshot_rgchze.jpg)

Check it out [here](https://jekflix.rossener.com/about/).

## 联系页面

模板中存在使用 Vue 创建的联系表单，因此您不必从头开始.

![Contact Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566476192/contact-page-screenshot_efux2y.jpg)

Check it out [here](https://jekflix.rossener.com/contact/).

## 404 error page

该模板还已经处理了 404 错误.

![404 Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566476323/404-page-screenshot_qiieyi.jpg)

Check it out [这里](https://jekflix.rossener.com/404/).

## Feed RSS

每次生成时都会自动生成一个源文件.

查看示例 [这里](https://jekflix.rossener.com/feed.xml).

## Disqus

*(Optional)*

Jekflix模板实现了Disqus插件，允许访问者在帖子中发表评论.

请参阅的 [文档](settings.md#disqus_username) 以对其进行配置。

##精选文章

*(Optional)*

在这个 2.0 版本中，英雄锁定被添加到主页，就像 Netflix 对电影所做的那样.

要打开/关闭此功能，请参阅 [文档](settings.md#show_hero).

![Page with hero screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566477681/page-with-hero-screenshot_ixyjzp.jpg)

## 主页分页

*(Optional)*

在主页中显示帖子有两种不同的选项，第一个是在向下滚动时加载新帖子，第二个是添加分页.

要添加分页，请参阅 [docs](settings.md#paginate).

## 帖子侧边栏

*(Optional)*

正如许多人所要求的，Jekflix模板2.0为帖子增加了一个可选的侧边栏。

要显示/隐藏边栏，请参阅 [docs](settings.md#two_columns_layout).

![Post with two columns screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566476793/two-columns-screenshot_phumrl.jpg)

## 分页帖子

*(Optional)*

您还可以通过分页帖子来提高广告浏览量。

要将帖子分成不同的页面，请参阅 [docs](post.md#paginate).

![Paginated Page Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566430021/paginated-page-screenshot_zx4xjn.jpg)

## “在你走之前”模式

*(Optional)*

为了让访问者对您的内容感兴趣，您可以在他们离开页面或/和他们到达帖子末尾之前向他们展示一些帖子推荐.

See the [docs](settings.md#show_modal_on_exit) for more information.

![Modal screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566478245/before-you-go-screenshot_prrplk.jpg)

## 帖子推荐

默认情况下，当访问者到达文章末尾时，所有帖子都会显示帖子推荐，例如:

![Recommendation Screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566478555/recommendation-screenshot_wzhchs.jpg)

Thi的功能应该类似于您完成电影或系列剧集时的 Netflix 推荐.

## 数学表达式

*(Optional)*

*Jekflix 模板 3.1.0* 现在通过以下方式支持数学表达式 [MathJax](https://www.mathjax.org/) library, thanks to **[@XieGuochao](https://github.com/XieGuochao)**.

您只需要 2 个步骤:

1. Set `math: true` for a post.
2. Adopt the _MathJax_'s grammar for $\LaTeX$.

For example, `$\sum_{i=1}{10} = 55$` will be rendered as <img src="https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,q_78,w_270/v1585835744/Screen_Shot_2020-04-02_at_10.55.24_uafb07.jpg" width="135">.

## Netlify CMS ready

*Jekflix模板2.0.0*的最新成员是Netlify CMS集成。

使用Netlify CMS，您将能够使用编辑器创建/编辑帖子，访问工作流程面板并通过单击更改博客的各个方面。

要使用Netlify CMS，您需要先完成一些步骤。请参阅的 [docs](netlify-cms.md#netlify-cms) for more info.

以下是一些屏幕截图:

![Netlify CMS post list screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-1_a0qezm.jpg)

![Netlify CMS post edition screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-2_aupygb.jpg)

![Netlify CMS workflow screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-3_bj5sks.jpg)

![Netlify CMS site settings screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-4_ycfqdp.jpg)

![Netlify CMS theme settings screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-5_k6dan9.jpg)
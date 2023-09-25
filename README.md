# Jekflix 主题模板

![Jekflix Template Cover Image](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1505354182/jekflix-logo_mfngps.png)

>在此处查看[实列](https://jekflix.rossener.com/).

## 这是什么？

>jekyll 主题灵感来自 Netflix （网飞）面板，适合喜欢电影和电视剧的人，它是一个酷炫外观的博客.

![Jekflix Screenshot Image](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566390829/jekflix-screenshot-2_zfiog2.jpg)

## 特征

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
- [RSS 地图](docs/features.md#feed-rss)
- [Disqus（可选）](docs/features.md#disqus) 
- [精选帖子（可选）](docs/features.md#featured-post) 
- [主页分页（可选）](docs/features.md#home-page-pagination)
- [帖子侧边栏（可选）](docs/features.md#posts-sidebar)
- [分页帖子（可选）](docs/features.md#paginated-posts) 
- [触发模式（可选）](docs/features.md#before-you-go-modal) 
- [帖子推荐](docs/features.md#post-recommendation)
- [Netlify CMS 发帖管理系统](docs/features.md#netlify-cms-ready)
- [翻译](docs/setup.md#translations) **new!**
- [数学表达式（可选）新增！](docs/features.md#math-expressions) **new!**

## 搜索引擎优化

- Google Analytics       / 谷歌分析
- Meta tags              / 元标记
- JSON-LD
- Sitemap.xml            / 网站地图.xml
- Social Media ready     /社交媒体就绪

## 快速安装

>如果您要安装到现有的 Jekyll 项目，请将此行添加到项目的`Gemfile`

```
gem "jekflix"
```

将此行添加到项目的： `_config.yml`:

```
theme: jekflix
```

然后运行：

```
$ bundle
```

或者自己安装为：

```
$ gem install jekflix
```

### 主题颜色

主题颜色目录 `/assets/css/styles.scss` 

```txt

$themeColor: #ff0a16;
$primaryDark: #141414;
$accentDark: #ffffff;
$lightGray: #f2f2f2;
$texts: #333333;

@import "jekflix";
```

>修改上面的颜色值可以更改主题颜色.

### 站点配置

您可以在项目中更改的一些属性，请查看 [文档](docs/settings.md#settings) 更改根目录下的`_config.yml`文件，它能自定义一些配置.

## 安装

>如果要克隆此存储库，请按照以下说明操作：

- [环境](docs/setup.md#environment)
- [安装模板](docs/setup.md#installing-template)
- [本地运行](docs/setup.md#running-local)

## 自定义

>请参阅 [设置文档](docs/settings.md#settings) 以自定义布局、标题、社交媒体等.

## 主题

>您可以通过更改文件轻松更改主题颜色 `src/yml/theme.yml`, 然后在您的终端中运行 `gulp build` .

## GitHub pages

>这是一个已知问题，将网站部署到 GitHub pages 时无法运行 gulp， 因此，您必须更改主题的颜色并在本地执行命令，`gulp build` 然后将更改推送到GitHub 仓库中，目前没有其他解决办法.
要查看部署网站时的外观，请在本地运行`gulp build`后，在访问. http://127.0.0.1:4000/

## 发布帖子

使用 `Markdown`[格式参看](docs/post.md#front-matter-properties) 创建帖子.

> **Note:** 注意：如果要克隆此存储库，可以使用可用[脚本](docs/post.md#creating-a-post)自动生成帖子.

## 问题？

>请提交  [GitHub 问题](https://github.com/thiagorossener/jekflix-template/issues/new).

## 许可证

>Jekflix 模板在 MIT许可证下可用.有关详细信息，请参阅[许可证](https://github.com/thiagorossener/jekflix-template/blob/master/LICENSE)文件. 

## 作者

[Thiago Rossener](https://rossener.com/)

Do you like my work? Buy me a coffee!

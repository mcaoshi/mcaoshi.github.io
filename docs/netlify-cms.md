# Netlify CMS

*Jekflix* 已准备好进行 Netlify CMS 集成，这意味着您可以创建/编辑帖子、作者、类别、主题等。无需接触一行代码！

但是，只有在克隆存储库时才能使用它。如果您使用的是“gem”，则需要自己在项目中设置 Netlify CMS。

## Deploy with Netlify

使用网络 [documentation](https://www.netlify.com/docs/continuous-deployment/) to set up *Continuous Deployment*.

设置“构建”命令时，请将其更改为“gulp build”。如果您已经部署了站点但忘记执行此操作，请按照以下步骤操作：

1. 转到顶部菜单并选择“**部署**”
1. 在“持续部署>生成设置”中，单击“编辑设置”**
1. 将“构建命令”更改为“吞噬构建”

就是这样。每次推送新提交时，您的项目都会生成和部署。

## Integrate with Netlify CMS

使用 Netlify 成功部署网站后，请按照 [启用身份和 Git 网关]（https://www.netlifycms.org/docs/add 到您的站点/#enable-身份和 git 网关）演练才能访问您的网站 CMS。

Some important things to keep in mind:

1. 通过“本地主机：3000/管理员”或“yourdomain.com/admin”在本地访问您的CMS
1. 可用的 CMS 数据**始终**从存储库中提取。这意味着，即使您在本地工作，CMS 也不会获得本地更改，直到您将它们推送到 GitHub 中。
1. 通过 CMS 发布的每个更改都将自动部署到生产环境，因此请谨慎发布的内容。
1.CMS允许您将数据保存为*草稿*，因此在您发布更改🙂之前，它不会进入生产环境

查看一些内容管理截图:

![Netlify CMS post list screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-1_a0qezm.jpg)

![Netlify CMS post edition screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-2_aupygb.jpg)

![Netlify CMS workflow screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-3_bj5sks.jpg)

![Netlify CMS site settings screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-4_ycfqdp.jpg)

![Netlify CMS theme settings screenshot](https://res.cloudinary.com/dm7h7e8xj/image/upload/v1566479287/netlify-page-5_k6dan9.jpg)
# 安装

## 环境

在开始之前，请确保您已安装 [Ruby](https://www.ruby-lang.org/en/documentation/installation/) 和 [NodeJS](https://nodejs.org/) .

然后安装 `Jekyll`:

```txt
$ gem install jekyll
```

安装 `Gulp` 客户端：:

```
$ npm install gulp-cli -g
```

## 安装主题模板

1. 克隆[ Jekflix 主题 ](https://github.com/thiagorossener/jekflix-template/fork)到你的github仓库，或者直接访问下载
2. 复制您刚刚克隆的 github 仓库 git 到本地:
```txt
$ git clone https://github.com/你的用户名/jekflix-template.git
```
2. 到 jekyll-template 主题目录下：
```txt
$ cd path/to/jekyll-template
```
3. 安装 npm 包：:
```txt
$ npm install
```
4. 安装 Ruby 依赖项：:
```txt
$ bundle install
```
5. 构建 Jekyll:
```txt
$ bundle exec jekyll build
```
6. 然后运行 Gulp:
```txt
$ gulp
```

## 在本地运行

完成上述步骤后，要在本地运行 Jekyll，您只需运行 Gulp:
```txt
$ gulp
```

## 定制

*Jekflix 模板允许您使用多种设置个性化您的网站。有关更多详细信息，请参阅[文档](settings.md#settings) .

对于高级主题自定义，请检查目录`_sass`中的样式文件

## 翻译

为了翻译整个主题中的文本，请在`src/yml`中创建`translations.yml`文件并添加以下设置。

> **注意：**如果您使用的是`gem`，只需将其添加到`_config.yml`中即可。

```
translations:
  text:
    new_post: "New Post"
    see_also: "See also"
    search: "Search"
    author: "Author"
    share: "Share"
    comments: "Comments"
  button:
    read_now: "Read Now"
    share_on_twitter: "Share on Twitter"
    share_on_facebook: "Share on Facebook"
  pagination:
    page: "Page"
    of: "of"
    next_page: "Next Page"
    next_post: "Previous Page"
  recommendation:
    text: "Why don't you read something next?"
    back_btn: "Go back to top"
  error_404:
    title: "Page not found :("
    message: "I'm sorry. We couldn't find the page you are looking for."
    image_alt: "404 - Page not found"
  contact:
    title: "Talk to me"
    subject: "New contact!"
    submit_btn: "Send"
    placeholders:
      name: "Your name"
      email: "Your e-mail"
      message: "Your message"
    errors:
      locale: "en"
      empty_name: "Name is required"
      empty_email: "Email is required"
      invalid_email: "Email is invalid"
      empty_message: "Message is required"
    after_send:
      title: "Message sent!"
      message: "Thank you for sending me a message. I'm going to answer ASAP."
```
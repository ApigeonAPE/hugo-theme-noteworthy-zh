# Noteworthy-zh

Noteworthy 是为作家和博主打造的极简 Hugo 主题，本分支版本已经汉化。[原仓库](https://github.com/kimcc/hugo-theme-noteworthy/)

![Noteworthy desktop screenshot](https://github.com/ApigeonAPE/hugo-theme-noteworthy-zh/blob/master/images/screenshot.png)


## 特性

* 完全响应
* 内置谷歌分析和 Disqus
* 支持 Ko-fi 捐赠按钮
* 语法高亮
* 支持 KaTex 数学公式
* 关于、标签和归档页面
* 内置RSS
* 可添加社交账户链接
* 支持SCSS
* 中文版独有的：不蒜子访问统计和知识共享(CC)协议

## 安装

切换至 Hugo 的根目录，克隆此存储库

```
git clone https://github.com/kimcc/hugo-theme-noteworthy.git themes/noteworthy
```
更多详细信息请见[Hugo官方文档](https://gohugo.io/getting-started/quick-start/)

## 帮助

详细帮助请见wiki

常见问题如：

* 如何关闭不蒜子
* 多语言
* 更改或弃用CC协议

## 图片画廊

要使用主题中内置的 `resize-image` 短代码制作画廊，您需要创建一个 [Post Bundle](https://gohugo.io/content-management/organization/#page-bundles)。 为您的画廊创建一个文件夹，将您的 Markdown 文件和图像放入其中，并将您的 Markdown 文件重命名为“index.md”。 例如：

```
my-new-post
- index.md
- image1.jpg
- image2.png
```

然后，您可以使用以下短代码在 Markdown 文件中添加图像： 

```
{{< resize-image src="image1.jpg" alt="My first image" >}}
```

像这样添加每个图片的标题： 

```
{{< resize-image src="image2.png" alt="My second image" caption="My caption" >}}
```

## “阅读全文”按钮

设置 config.toml 中的`showReadMore = false` 成 `true` 来在主页的摘要下方显示 “阅读全文” 按钮。

## 社交账户链接

在 `config.toml` 文件的 `params` 中，您可以添加您的社交帐户链接。 只需删除或注释掉您不想包含的内容所在的行，它们的图标就会从网站上消失。 

```
# 主要

# 下面的例子演示了如何显示一个图标:
email = "*********@qq.com" # 邮箱地址

weibo = "#" # 微博
# 以下的国内不常用

# 下面的例子演示了如何隐藏一个图标:
# facebook = "#" # 注释掉
                 # 或删除掉

twitter = "#" # 推特，需要科学
instagram = "#" # Meta旗下照片墙，需要科学
tumblr = "#"
reddit = "#"
pinterest = "#"
youtube = "#" # 油管，需要科学
vimeo = "#"
vk = "#"
linkedin = "#"

# 写作
medium = "#"
blogger = "#"
wordpress = "#"

# 视觉设计
dribbble = "#"
behance = "#"
deviantart = "#"
flickr = "#"

# 音乐
soundcloud = "#" # 音云

# 编程
github = "#"
stackoverflow = "#"
gitlab = "#"
codepen = "#"

# 学术
googlescholar = "#" # 谷歌学术
impactstory = "#"
orcid = "#"

# 旅行
googlemaps = "#" # 谷歌地图
tripadvisor = "#"
```


## Disqus 和谷歌分析

在`config.toml`中添加你的 Disqus ID 和谷歌分析标识符：

```
# 在这里添加你的 Disqus ID.
disqusShortname = ""

# 在这里添加你的谷歌分析标识符，格式: UA-XXXXXXXX-X
googleAnalytics = ""
```

## Ko-fi 捐赠按钮

如果你想在博客中启用 Ko-fi 捐赠按钮, 在 `config.toml`中添加你的ID：

```
# 把“enableKofi”设置为 true 来启用 Ko-fi 捐赠按钮. 添加你的 Ko-fi ID 来链接到你的账户。
enableKofi = true
kofi = ""
```


## License

使用 [MIT 许可证](https://github.com/ApigeonAPE/hugo-theme-noteworthy-zh/blob/master/LICENSE.md).

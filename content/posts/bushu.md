---
categories:
- 随笔
date: '2022-04-06T00:10:00.000Z'
showToc: true
tags:
- 学习
- 总结
- 编程
title: 部署成功总结

---



用了两周时间，终于把网址成功部署到GitHub上了。

- [https://samhawthorne.github.io/](https://samhawthorne.github.io/)

这是网址↑↑↑

总结一下部署的过程：

1. 先在本地创建hugo文件夹。下载hugo包到本地，新建bin和sites两个文件夹。把hugo压缩包里的文件全部解压到bin文件夹里面。

1. 下载主题。用代码下载。

1. 配置config.yml文件。

1. 新建.github workflows两个文件夹。

1. 配置自动化部署文件。notion_to_blog.yml和gh_pages.yml。

1. 配置自动化脚本deploy.sh。

1. GitHub部署。

1. 公钥密钥配置。

1. [automate.io](http://automate.io/)配置。

1. notion数据库配置。

1. notion API 配置。notion database id配置。

1. 打开git bash。

1. 同步本地和在线代码文件。git pull --rebase origin develop。

1. 运行自动化脚本deploy.sh。bash deploy.sh。

1. 查看GitHub Action运行结果。

1. 排查bug。

1. 在notion写文章。

1. automate自动获取api同步到GitHub。只有新的一行automate才会读取。如果是更新原来的文章，需要手动在GitHub提交issue：notion-ci。

1. GitHub自动运行两个yml脚本，把notion内容转成md文件，再将md转成html，最后部署网页。



![](https://raw.githubusercontent.com/SamHawthorne/pic/master/notionimg/f6/95/f695d725f474c08fbfbbdfb0f97fe377.png)

![](https://raw.githubusercontent.com/SamHawthorne/pic/master/notionimg/53/48/5348b47a8669a21bf3d2c10c3bf96a56.png)



未完待续......



参考链接：
[『手把手』利用 Github Actions 轻松部署 Hugo 博客_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1x7411q7R9)

[用 Hugo 配合 Github Actions 自动构建我的博客 - Blog My Life (nashome.cn)](https://www.nashome.cn/posts/hugo-github-actions/)

[notion实现自动发布到hugo github博客 - Akkuman - 博客园 (cnblogs.com)](https://www.cnblogs.com/Akkuman/p/15672566.html)

[notion实现自动发布到hugo github博客 | Akkuman 的博客 (hacktech.cn)](https://hacktech.cn/2021/12/10/notion-to-github-blog/)




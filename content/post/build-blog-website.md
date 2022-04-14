---
title: "Hugo+Even搭建个人博客"
date: 2022-04-12T21:55:35+08:00
lastmod: 2022-04-13T23:41:21+08:00
draft: true
keywords: []
description: ""
tags: []
categories: []
author: ""

# You can also close(false) or open(true) something for this content.
# P.S. comment can only be closed
comment: false
toc: false
autoCollapseToc: false
postMetaInFooter: false
hiddenFromHomePage: false
# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: false
reward: false
mathjax: false
mathjaxEnableSingleDollar: false
mathjaxEnableAutoNumber: false

# You unlisted posts you might want not want the header or footer to show
hideHeaderAndFooter: false

# You can enable or disable out-of-date content warning for individual post.
# Comment this out to use the global config.
#enableOutdatedInfoWarning: false

flowchartDiagrams:
  enable: false
  options: ""

sequenceDiagrams: 
  enable: false
  options: ""

---

这是我博客的第一篇文章，主要讲解基于框架hugo和主题even，在本地搭建博客的详细步骤。

<!--more-->

{{% music "569214250" %}}

### 1. 安装hugo

brew install hugo

### 2. 创建站点

hugo new site website 

### 3. 配置主题

cd website  
git clone https://github.com/olOwOlo/hugo-theme-even themes/even  
cp themes/even/exampleSite/config.toml ./  
cp themes/even/archetypes/default.md ./archetypes/  

### 4. 修改配置

|  属性   | 值  |
|  ----  | ----  |
| title  | "strubert's blog" |
| name  | "strubert" |
| logoTitle | "飞鸟" |
| a-email | "mailto:strubert@qq.com" |
| g-github | "https://github.com/jimmyforrest" |
| ... | ... |

### 5. 新建文章

hugo new post/build-blog-website.md

### 6. 本地调试

hugo server -D

### 7. 相关参考
+ [Hugo](https://gohugo.io/getting-started/quick-start/)  
+ [hugo-theme-even](https://github.com/olOwOlo/hugo-theme-even)  
+ [Hugo + even + GitHub Pages+ Utterances搭建个人博客](https://blog.csdn.net/perfumekristy/article/details/122070579)



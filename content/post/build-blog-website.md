---
title: "Hugo+Even搭建个人博客"
date: 2022-04-12T21:55:35+08:00
draft: true
---

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

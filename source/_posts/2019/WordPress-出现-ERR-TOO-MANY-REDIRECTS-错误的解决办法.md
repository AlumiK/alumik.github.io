---
title: WordPress 出现 ERR_TOO_MANY_REDIRECTS 错误的解决办法
categories: 其他软件问题
tags: WordPress
abbrlink: 10
date: 2019-06-24 15:38:11
---
一种解决方法是指明网站入口文件为 *index.php* 。

具体到 Apache2 ，修改网站的配置文件，添加：

```apache
<Directory /var/www/example>
    DirectoryIndex index.php
</Directory>
```

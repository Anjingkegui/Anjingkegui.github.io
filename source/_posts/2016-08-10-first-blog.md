---
title: 好了，搭建好自己的主页了！
date: 2016-08-10 22:05:56
category:
- Hexo
tags:
- Hexo
- 搭建博客
---
初步调研了一下，决定采用hexo来搭建自己的博客，选了层次分明的主题jacman，好了，开工。
<!-- more -->
### 安装 ###
- 先安装[Node.js](https://nodejs.org/en/)
- Git Shell
- 建立存放博客源文件的文件夹，并通过Git Shell进入到该文件夹下：

```
	npm install -g hexo
	hexo init
```

或

```
	hexo init
	npm install
```

都是可以的。接着：

```
	npm install hexo-deployer-git --save
```

装主题：

```
	git clone https://github.com/wuchong/jacman.git themes/jacman
```

就好了。换台电脑也是同样的操作，注意备份一些文件即可。

### 配置 ###
- 配置hexo，配置主题外观（配色、图片、字体等等）
- 个人信息中的font图标加入qq和微信
- 配置多说的样式
- 配置cnzz统计
- 配置sitemap

目前还存在的问题：
- 站内搜索
- 百度检索不到页面
- totop

### 使用指南 ###
- `Markdown`语法自然是没问题。但是由于对代码高亮的支持，在写代码的时候注意可以加入[语言](http://highlightjs.readthedocs.io/en/latest/css-classes-reference.html)。

![插入代码时的写法](http://oboo3frns.bkt.clouddn.com/20160811145331.png)

效果如下：

``` c
	#include <stdio.h>
	
	void main()
	{
		ptintf("Hello World!");
		return;
	}
```

- 每次要发布新的博文时，直接到`blog`文件夹下：

```
	hexo new ***  // *** 指代文件系统中该文件的标题，前面自动会加上日期，不用担心重名
	
	// 去编辑md文件

	hexo clean  // 清理
	
	hexo s  // 开启本地预览

	hexo g -d  // 生成和发布
```

### 参考的文章 ###
[胖逆的嘟嘟关于Hexo的博客](http://www.cnblogs.com/tengj/category/809716.html)

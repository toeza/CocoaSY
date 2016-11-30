---
layout: post

title:  Toeza手机端内嵌Khtogel
date:   2016-11-30 10:32:42 +0800

categories: SEO
tag: [开发]

---

* content
{:toc}


# 描述 #


1.	toeza.com是一个网站，分PC端与手机端，所使用后台为[Dede](http://www.toeza.com/)

2.	khtogel.com也是一个网站，分PC端与手机端，点击进入[khtogel](http://khtogel.com/)

3.	toeza.com的PC端界面中已经内嵌了khtogel.com的PC端界面

4.	toeza.com的手机端界面中还未内嵌khtogel.com的手机端界面

	![toeza]({{ "/styles/images/Post/Figure1_1 toeza.png" | prepend:site.baseurl}})



	<table>
	<tr>
	<td><img src="{{ "/styles/images/Post/IMG_0206.PNG" | prepend:site.baseurl}}" width="50px" height="150px"></td>
	<td><img src="{{ "/styles/images/Post/IMG_0205.PNG" | prepend:site.baseurl}}" width="50px" height="150px"></td>
	</tr>
	</table>


# 目的 #


在toeza.com的手机端界面中还未内嵌khtogel.com的手机端界面


# 分析 #

1.	分析手机模板所在文件

2.	参考资料：
	
	1.	dedecms织梦生成wap手机模板的一些问题总结 
	[点击查看](http://jingyan.baidu.com/article/a24b33cd74e5db19ff002b69.html)


## 问题分析 ##
1.	未找到手机所在模板文件夹：templets/wap/(手机模板目录)


# 步骤 #

1.	安装本地DedeCMS进行测试，安装测试版本为： 
	[DedeCMS-V5.7-UTF8-SP1.zip](www.pcdd286.com/DedeCMS-V5.7-UTF8-SP1.zip)

	本地当前IP是：192.168.1.107

	后台测试目录：[点击进入](http://localhost/DedeCMS/uploads/dede/login.php?gotopage=%2FDedeCMS%2Fuploads%2Fdede%2F) 
	前台测试目录：[点击进入](http://localhost/DedeCMS/uploads/index.php?upcache=1)

2.	测试手机端模板所在目录

	PC端模板所在目录为：templets/default
	
	手机端首页加载路径：/m/index.php
	手机端栏目加载路径：/m/list.php?tid=(*)(example:tid=6)
	手机端文章加载路径：/a/pics/2010/0407/95.html

3.	分析"/m/index.php"文件
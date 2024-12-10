# 乌班图初始配置简短教程
本篇主要介绍的是在一个**完全干净**的ubuntu上进行相对简单的配置

前置知识：Linux的基本语句操作、一定的计算机基础

配置包括以下几个方面：
## 0.如何搜索教程
### 抛弃CSDN
首先，排除`CSDN`这个选项，因为这个平台又垃圾又难看

可以在每次搜索的字段后面添加`-csdn`，排除所有有关的搜索
### 精准搜索
其次，注意搜索的时候寻找和自己的环境相匹配的教程

比如你需要搜索：“乌班图环境下如何下载vscode？”这个问题，关键词可以是这样的：

Ubuntu22.04 下载 vscode

注意一定要在提问的时候添加对应的环境版本，不同版本的某些操作是不兼容的
### 寻找高质量教程
尽量选择比较完整的教程观看，博客园、知乎都是不错的

希望你在每个教程都不会出现问题

如果出现问题，解决问题或者更换教程都是很麻烦的事情
### 下文的食用提醒
操作1和2都是必须在开发机，即你的Linux或者Ubuntu或者虚拟机上操作的

操作3是在自己的机子上，不用在虚拟机上操作，当然可以在开发机上继续操作（我没试过）
## 1.下载vscode并且配置python
此步骤对于本次实验没什么作用，可以跳过直接看第2步。
## python下载
Ubuntu自带python3，所以python一般不需要下载

可以通过如下指令查看：
```
python3 --version
```
如果出现问题，请自行搜索下载方法

## vscode下载以及python配置
与Windows下的vscode配置差不多

[官网](https://code.visualstudio.com/download)

下载.deb文件，并且自行搜索操作deb文件的指令后完成下载，应该可以从任务栏中找到图形界面，进行安装即可

在下载完vscode之后，在左侧的**扩展**一栏中添加扩展，包括但不限于：

`Chinese`, `python`

下载完后，新建python写个hello world，运行时选择python解释器即可

## 2.配置docker
我参考的是这份教程:

[Ubuntu下载docker](https://www.runoob.com/docker/ubuntu-docker-install.html)

其中在最后一步前没有什么问题，把所有的操作都复制粘贴一下即可，选择版本的那一步记得把`<VERSION_STRING>`字段替换

最后一步你会遇到docker无法run的情况，这是因为官方的docker镜像被墙了，没法运行，请自行百度寻找国内能用的镜像源

当然如果您有能力，可以选择给docker挂代理的方式，比如使用`clash`等软件，这里就不赘述了

## 3.数据库可视化

我选用的是HeidiSQL进行可视化，当然navicat、MySQL workbench都是可以的

在连接数据库时，可以参考这篇文章：

[数据库可视化](https://zhuanlan.zhihu.com/p/687413801)
## 4.配置ssh
如果您有远程开发的需要，可以自行搜索ssh以及相关操作进行配置

这里推荐vscode的ssh插件`Remote-SSH`，个人体验极佳
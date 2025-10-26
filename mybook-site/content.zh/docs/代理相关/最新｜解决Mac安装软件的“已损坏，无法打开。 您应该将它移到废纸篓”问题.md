---
title: "最新｜解决Mac安装软件的“已损坏，无法打开。 您应该将它移到废纸篓”问题"
source: "https://zhuanlan.zhihu.com/p/135948430"
author:
  - "[[huazai终身学习]]"
published:
created: 2025-10-26
description: "一、允许“任何来源”开启苹果从macOS Sierra 10.12 开始，已经 去除了允许“任何来源”的选项，如果不开启“任何来源”的选项，会直接影响到无法运行的第三方应用。所以开启“任何来源”的方法如下： 打开【启动…"
tags:
  - "clippings"
---
![最新｜解决Mac安装软件的“已损坏，无法打开。 您应该将它移到废纸篓”问题](https://pic1.zhimg.com/70/v2-14318d1da9cb9c545a541457cd1b2936_1440w.avis?source=172ae18b&biz_tag=Post)

最新｜解决Mac安装软件的“已损坏，无法打开。 您应该将它移到废纸篓”问题

![](https://pic3.zhimg.com/v2-5b81946b01c8285aab0296f6ac040718_1440w.jpg)

一、允许“任何来源”开启 苹果从 macOS Sierra 10.12 开始，已经 去除了允许“任何来源”的选项 ，如果不开启“任何来源”的选项，会直接影响到无法运行的第三方应用。 所以开启“任何来源”的方法如下： 打开【启动台】，选择【 终端 】，输入： sudo spctl --master-disable 然后回车，继续输入密码（密码输入时是不可见的），然后回车。 接着打开【系统偏好设置】，选择【 安全性与隐私 】，选择【通用】，可以看到【任何来源】已经选定。 接着打开文件进行安装。 二、发现还是显示“已损坏，无法打开。 您应该将它移到废纸篓”，不急，接下来用这种方法： 在终端粘贴复制输入命令（注意最后有一个空格）： sudo xattr -r -d com.apple.quarantine 先不要按回车！先不要按回车！先不要按回车！先不要按回车！ 然后打开 “ 访达 ”（Finder） 进入 “应用程序” 目录，找到该软件图标，将图标拖到刚才的终端窗口里面，会得到如下组合(如图所示)： sudo xattr -r -d com.apple.quarantine /Applications/WebStrom.app 回到终端窗口按回车，输入系统密码回车即可。 接着重新打开安装软件，就可以正常安装了。 注：如果试了还是不行，那就只能下载以前的版本了。

发布于 2020-04-24 15:21[Mac](https://www.zhihu.com/topic/19550264)[Mac OS X 使用技巧](https://www.zhihu.com/topic/19591970)[macOS](https://www.zhihu.com/topic/19550290)

写下你的评论...

233 条评论

默认

最新

[河广](https://www.zhihu.com/people/9e7aa80a68c65283a96a3d25e0d8b6b7)

sudo xattr -r -d com.apple.quarantine 今天测试这条命令说 -r 不支持，去掉-r可以

2023-03-31

[船长谢尔曼](https://www.zhihu.com/people/fc670f0f0ef5fa9d111c65cd2edf1fb0)

还可以试试这条更新的：sudo xattr -rd com.apple.quarantine (拖入APP）+回车在输入密码，OK！

2024-10-24

[梁间燕喃](https://www.zhihu.com/people/c44c4f6cbf7e0a1f01475e15f2adee72)

[船长谢尔曼](https://www.zhihu.com/people/fc670f0f0ef5fa9d111c65cd2edf1fb0)

为什么我这回车不用密码？

03-24

[铅笔](https://www.zhihu.com/people/f025b051d96a1e2d2e7c4855d8f07e3a)

navicat不行，os13

2022-12-24

[老那一头秀发](https://www.zhihu.com/people/4912ac610c6c4c2e369550bf7fb72d02)

Not enough arguments for option -d. Expected at least 2 but got 1

2023-08-28

[拎壶冲](https://www.zhihu.com/people/fb415ebec2acf1993d9a13bd79ae2d1b)

你的App路径有空格，比如/Applications/Mi Home.app要换成/Applications/Mi\\ Home.app

2024-02-01

[寒江雪](https://www.zhihu.com/people/b5918cf39f24a14e3cbaa723ddb11919)

sudo xattr -r -d com.apple.quarantine /pathfolder  
后面是你文件的路径:例如：/Applications/xxxx.app

2024-01-17

[FlynnAI](https://www.zhihu.com/people/896ac6285d681116c92445733315db08)

牛逼，用来解锁yesplaymusic

2021-07-18

[橡皮擦](https://www.zhihu.com/people/3076864a8f4677924b201d81d6db76a3)

牛牛牛，小母牛坐火箭回家——牛逼到家了

2021-10-26

点击查看全部评论

写下你的评论...

set 限制解除 

x1.00

\>

<

\>>

<<

O

x1.00
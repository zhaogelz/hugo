1、必须在win的笔记文件夹下执行: `git config core.fileMode false`  #不要检查权限变化
因为安卓和win文件夹权限不同,不这么设置,即使你没有任何改动,由于文件的操作权限变了，也会自动视为更改了全部文件，极易造成冲突，且影响同步速度。

2、[点击下载该文本文件](.gitignore)
obsidian git是gitee登陆,不是github,github密码失效,要通过开发者中心(头像->设置->最下方开发人员)创建令牌登陆(注意给权限),github更新无法用密码登陆了




.gitignore和我这同步，不然容易出现冲突

改了gitignore，要清理提交缓存git rm -r --cached .
git add .

安装：obsidian  https://github.com/obsidianmd/obsidian-releases/releases  安装插件
1.安装git： https://git-scm.com/downloads/win
2.访问gitee: https://gitee.com/

github已经无法密码登陆，可以创建令牌，用令牌替换密码
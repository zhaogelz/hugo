搭建服务器（基本使用）：https://zhuanlan.zhihu.com/p/45510637
 
在本地新建远程仓库：1、参考上文“ 搭建服务器”，但不禁用git账户的shell  
2、在本地登录远程git账户，本地终端执行：ssh git@服务器IP  
3、参考上文“ 搭建服务器”里的新建空白仓库，如（git init --bare /git/text）  
4、建好后就可以将远程仓库与本地仓库关联了（假如新建了多余的远程仓库记得删了rm -rf 文件夹路径）
 
使用时注意当前在哪个分支的哪个提交
 
整理提交之合并提交：鼠标右键（选择早期提交）-》交互式变基-》选择较新的一个-》用此前的squash（会将最相邻的合并）-》编辑信息-》确定  
（通过拖拽的方式合并容易有莫名其妙的错误）
 
整理提交之合并提交：与上条类似，需注意，一旦删除某个提交，其中所做的更改也会消失，所以不建议用，建议改为使用合并
 
放弃本地更改：先回滚到早期版本，再拉取
 
有文件暂时不想提交到远程，但之后可能提交：贮藏
 
==sourcetree====使用：====https://zhuanlan.zhihu.com/p/533052453==
 
忽略文件：https://www.toptal.com/developers/gitignore  
[https://blog.csdn.net/ananlele_/article/details/115060102](https://blog.csdn.net/ananlele_/article/details/115060102)
 
强制删除远程提交：切换到要保留的分支，进入git bush，强制提交：  
git push -f  
参考：https://www.jianshu.com/p/6c32b768a31a
 
整理历史提交（注意只整理远端没有的提交）：https://www.jianshu.com/p/9e91ed38e74a
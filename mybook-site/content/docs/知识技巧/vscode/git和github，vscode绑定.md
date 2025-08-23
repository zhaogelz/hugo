大致流程，1、在系统用git生成ssh密钥  
2、添加SSH密钥到SSH代理（eval "$(ssh-agent -s)" ssh-add ~/.ssh/id_rsa ）  
3、然后在github网站里填入密钥。  
4、测试连接：ssh -T git@github.com  
然后就可以通过vscode拷贝存储库定了==（====vscode====拷贝存储库最好先翻墙，不然可能报错）==
   

==注：默认无法同步超过====100m====同步大文件，搜索== ==GH001: Large files detected====”== ==错误信息== ==解决（====https://segmentfault.com/a/1190000045394658====）==
 
==git====插件使用==

![Exported image](png/Exported%20image%2020250821052707-0.png)
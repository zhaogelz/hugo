V2rayA方案弃用，不支持vless协议。改用xray  
Xray [https://github.com/XTLS/Xray-core](https://github.com/XTLS/Xray-core)  
1、下载项目文件后解压。在从可用机器导出配置到文件夹，并命名1.json  
2、终端执行：./xray -c 1.json  
3、新开终端，设置当前终端代理==（====docke====拉取镜像这样可能无效，需要在配置文件处代理）==  
export ALL_PROXY="http://127.0.0.1:10808"  
4、测试：返回梯子ip  
curl -x socks5://127.0.0.1:10808 https://ifconfig.me  
curl [https://ifconfig.me](https://ifconfig.me)  
（桌面系统，软件要通过代理，可以去系统的网络设置那里配置代理服务器）
 
V2rayA： [https://github.com/v2rayA/v2rayA](https://github.com/v2rayA/v2rayA)  
[https://snapcraft.io/v2raya](https://snapcraft.io/v2raya)  
注意：要在管理页面的设置里设置代理模式才能使用 设置-\>不尽兴分流-\>redirect(trojan可用vless不可用)
 
管理页面：http://localhost:2017/  
用户名：root  
密码：123456780
 
用法：先勾选节点-》再左上角 就绪（启动）
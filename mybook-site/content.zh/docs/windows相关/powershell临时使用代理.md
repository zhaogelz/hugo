本地代理端口为10808的情况下
 
$env:HTTPS_PROXY = "[http://127.0.0.1:10808](http://127.0.0.1:10808)"  
$env:HTTP_PROXY = "[http://127.0.0.1:10808](http://127.0.0.1:10808)"
 
linuxshell：参考 [https://zhuanlan.zhihu.com/p/153124468](https://zhuanlan.zhihu.com/p/153124468)  
获取ip：cat /etc/resolv.conf
 
export ALL_PROXY="http://172.20.64.1:10808"
 
验证生效：curl [http://ifconfig.me](http://ifconfig.me)  
curl -x socks5://127.0.0.1:10808 [https://ifconfig.me](https://ifconfig.me)
 
也可用笔记linux相关 Ubuntu 代理vpn（s）
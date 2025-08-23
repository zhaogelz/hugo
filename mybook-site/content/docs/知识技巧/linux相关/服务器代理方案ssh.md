1. 网络来源服务器SSH配置  
登录服务器查看 /etc/ssh/sshd_config 关键参数：
 
PermitRootLogin yes # 必须允许root登录  
PasswordAuthentication yes # 启用密码验证  
AllowTcpForwarding yes  
修改后需重启SSH服务：systemctl restart ssh
 
2、使用网络服务器ssh方式：  
# 1. 开启隧道（当前终端）（输入密码后阻塞，另开窗口执行2）  
显示详细调试信息ssh -vvv -N -D 127.0.0.1:39001 root@144.34.232.235  
ssh -N -D 127.0.0.1:39001 root@144.34.232.235  
强制使用ip4 ssh -4 -N -D 127.0.0.1:39001 root@144.34.232.235  
# 2. 设置终端代理==（====docke====拉取镜像这样可能无效，需要在配置文件处代理）==  
export ALL_PROXY="socks5://127.0.0.1:39001"  
powershell下（默认不支持socks5，得用powershell7，微软商店可安装）：$env:ALL_PROXY = "socks5://127.0.0.1:39001"
 
这两条估计不生效：$env:HTTPS_PROXY = "socks5://127.0.0.1:39001"  
$env:HTTP_PROXY = "socks5://127.0.0.1:39001"
 
# 测试代理功能  
curl -x socks5://127.0.0.1:39001 [https://ifconfig.me](https://ifconfig.me)  
curl [https://ifconfig.me](https://ifconfig.me)  
curl -4 [https://ifconfig.me](https://ifconfig.me)  
# 4. 使用完毕后按Ctrl+C终止隧道  
# 5. 取消代理（或直接关闭终端）  
unset ALL_PROXY
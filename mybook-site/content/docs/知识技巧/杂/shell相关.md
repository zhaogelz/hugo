xshell连串口：新建回话-》SERIAL-》选择串口和波特率
 
xshell连接模组 telnet协议 用户名root 密码：HDZW892226  
模组密码在：/xmlfile/sysInfoCfgEx  
dmesg命令查看有没有被kill，若有程序被杀死重启，打印能看到kill  
free显示还有多内存  
Kill 杀死线程  
ps查看线程
 
挂载（客户端执行）：mount -t nfs -o nolock 192.168.2.123:/NFS /nfsroot  
取消挂载：umount /nfsroot
 
模组守护进程：Daemon.sh
 
Ev300交叉编译工具：arm-himix100-linux-gcc  
Dv300交叉编译工具：arm-himix200-linux-gcc
 
运行sh脚本命令：sh ./文件名
 
写shell脚本注意空格，空格会影响语句结果
 
判断文件或文件夹是否存在：https://blog.csdn.net/u012206617/article/details/118366597
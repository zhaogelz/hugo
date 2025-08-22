重命名：f2  
指定文件夹打开终端：shift+鼠标右键（文件夹左上角单击文件可以用管理员打开）  
打开cmd：搜索cmd，进入位置，再右键管理员打开。  
截图:Win+ shift+s  
==ctrl + shift + delete== 快速清除浏览器缓存

\> ==清屏：====ctrl+l====或者====clear==   \> ==Win+I== ==控制面板==   
host位置：c:\windows\system32\drivers\etc
 
开机自启动文件夹：1、win+R，运行框输入shell:startup
 
2、C:\Users\engineer_e11\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup（注意\ray是我自己用户的用户名，大家复制粘贴时要改为你们自己的用户名）
 
C:\Users\朝歌\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup
 
管理员打开cmd（直接任务栏搜索cmd，右键管理员打开），切换路径示例：cd /d C:\Program Files
   

搜索输出CMD 管理员运行  
“sc config i8042prt start= disabled”并回车即可禁用笔记本键盘，要重启。  
输入“sc config i8042prt start= auto”恢复笔记本键盘功能。
   

一小时后关机：Shutdown -s -t 3600
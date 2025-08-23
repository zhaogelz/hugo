我也出现该问题，同时发现win系统的wsl也损坏了。1、通过该工具修复了wsl：https://github.com/microsoft/WSL/releases  
2、卸载docker desktop（尝试迁移，仍有问题），重装docker desktop后先升级，升级完成后，退出docker desktop。  
迁移镜像位置，先终端执行  
wsl --export docker-desktop D:\docker\docker-desktop.tar  
wsl --unregister docker-desktop  
wsl --import docker-desktop D:\docker\docker-desktop D:\docker\docker-desktop.tar  
后在docker desktop，设置-》Resources-》Advanced-》Disk image location修改镜像位置到固态盘D:\docker\DockerDesktopWSL（怀疑原本迁移不完善，或在机械盘唤起过慢导致）。  
补充：重装wsl，重装docker desktop都试过，均无效。按上文操作才好。
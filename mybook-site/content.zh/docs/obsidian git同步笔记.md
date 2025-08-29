## 下载访问链接：
> 1、obsidian  https://github.com/obsidianmd/obsidian-releases/releases  
> 2、安装git： https://git-scm.com/downloads/win
> 3、访问gitee: https://gitee.com/
> 4、此出提供我下载好的1、2链接安装包和.gitignore文件，可直接下载： http://xz.15390974.xyz/#/?code=700YK  

## 视频已提到但易忽略
1、Gitee必须配置ssh，作用是将你电脑设为信任设备，免输入用户名，密码即可上传文件。有未知问题，导致电脑端输入密码无法同步，故必须。

2、必须在win的笔记文件夹下执行: `git config core.fileMode false`  #不要检查权限变化
因为安卓和win文件夹权限不同,不这么设置,即使你没有任何改动,由于文件的操作权限变了，也会自动视为更改了全部文件，极易造成冲突，且影响同步速度。

3、直接下载拉到文件夹也行。[点击下载.gitignore](.gitignore)
在笔记文件夹下创建.gitignore文件（注意：开显示隐藏文件和后缀名），用于忽略不同设备的配置文件，我这个适配安卓和win，别的设备可能还需适当修改。
```
# 忽略 Obsidian 缓存与临时文件
.obsidian/cache/

.obsidian/workspace.json

.obsidian/workspaces/

.obsidian/trash/

# 忽略插件生成的缓存数据（如 Git 插件历史记录）
.obsidian/plugins/obsidian-git/data.json   # [[1][5][11]()

# 忽略系统文件
.DS_Store
Thumbs.db
desktop.ini

# 忽略备份文件
*.bak
*.tmp

# 忽略附件文件夹（按需启用）
# attachments/

# 特殊配置：保留核心插件配置（可选）
!.obsidian/plugins/  # 保留插件目录
!.obsidian/themes/   # 保留主题目录

# Ignore Smart Environment folder
.smart-env
.obsidian/plugins/recent-files-obsidian/data.json
.obsidian/workspace-mobile.json
.trash/
```

4、<font color="#c00000">（非必须，但执行了以防万一）视频内容补充：添加gitignore后，或gitignore添加了新内容后，要清理提交缓存，进入笔记目录（键盘shift不放，同时鼠标右键，找到在此处打开powershell）执行如下代码。</font>
```
git rm -r --cached .
git add .
```
<font color="#c00000">代码执行完，再进行一次手动同步</font>

5、手机中可能找不到同步按钮，按我视频中方法操作即可

## 额外记录
1、若不采用gitee而采用github，由于github密码即将失效,要通过开发者中心(头像->设置->最下方开发人员)创建令牌(注意给权限),用令牌取代密码
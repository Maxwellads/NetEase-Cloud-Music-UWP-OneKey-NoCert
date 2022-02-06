# 声明&比较

这是一个从 (https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack) Fork而来的分支，仅提供网易云一键安装脚本。部分内容被编辑以适应实际需要。

此项目对于原Fork有如下区别：

1、安装方式不同。本项目安装使用开发人员功能，无需安装证书；

2、文本帮助更加详细，更适合小白（？）；

3、就这些

# 简介

网易云音乐 UWP 重打包版，不会自动更新到 Win32 版。

注意：禁用Microsoft Store的自动更新功能是必要的，否则将会自动更新并且覆盖安装。

# 下载
[一键安装脚本+安装包](https://github.com/Maxwellads/NetEase-Cloud-Music-UWP-OneKey-NoCert/releases/download/Release/NCM-Onekey-NoCert.7z)

# 安装说明

1. 到 设置 > 更新与安全 > 开发人员设置 中，启用开发人员模式。
3. 解压下载的文件到桌面。
4. 确定你的设备处理器指令集类型。打开 设置 > 系统 > 关于，查看“系统类型”；如，“64位操作系统，x64架构处理器”，则运行脚本“Install-x64.bat”。
5. 本脚本仅在x64设备上测试。若安装了错误的架构，则脚本将自动退出。

# 无法登录的解决方案

请选择以下其中一种方法：

**[方法一（推荐）：](https://www.bilibili.com/read/cv9556360/)**

1. 点击 左下角“未登录”头像 → 关于网易云音乐，来到关于界面

2. 对界面右上角的网易云音乐 Logo 连续单击5下，然后迅速右击，会弹出调试对话框（如果不行则多试几次）

3. 将对话框中的服务地址 ```http://music.163.com``` 中的 ```http``` 改为 ```https```，即改为 ```https://music.163.com```，然后确认

4. 重启应用后登录

- [查看动图演示](https://i0.hdslb.com/bfs/article/5a5c6a3e97209bdc94e9a8440c7a4abff93fcb72.gif)

**方法二：**

1. 点击 发现音乐 → 最新音乐，此时“我喜欢的音乐”会出现在应用左栏

2. 点击 创建的歌单 → 我喜欢的音乐 → “未登录”头像，然后登录

- 注：应该只支持网易账号和手机号

# 进阶：本地回环代理设置

（如果你不知道这是做什么的，那么请忽略这一项）

管理员命令行运行：

`checknetisolation loopbackexempt -a -n="1f8b0f94.122165ae053f_kq4t7q4nstjby"`


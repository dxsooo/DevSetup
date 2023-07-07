0 （以macos 12为基础）
- 更新系统到最新
- 设置触控板
    - 【系统偏好设置】- 【触控板】- 【光标与点按】，打开【轻点来点按】
- 配置网络
- 从dock移除不常用的应用

1 终端配置
- 将终端从启动台的其他集合拉出到启动台，并加到dock中
- 将终端默认shell设置为 zsh
    - 【终端】- 工具栏【偏好设置】- 【通用】- shell的打开方式 - 命令：/bin/zsh
- 安装oh-my-zsh
    - 参考官网 https://ohmyz.sh/ ，选用 curl 方式（git会同时被下载安装）
    - 设置主题，修改 ~/.zshrc 文件中的 ZSH_THETE="kphoen"

2 VPN配置
这里使用 ClashX
- 从官方渠道下载：https://github.com/yichengchen/clashX/releases
- 配置：
    - 添加VPN配置文件：【配置】- 【托管配置】- 【管理】- 【添加】，url从VPN供应商获取
    - 增加规则：【配置】- 【更多设置】- 【忽略这些主机】，增加不需要走代理的域名
- 根据需要设置为系统代理
- 根据需要设置为开机启动

3 VScode 配置
官方渠道下载：https://code.visualstudio.com/
下载后将app拉入【应用程序】
打开程序并通过命令面板选择 在PATH中安装code命令

插件安装：
- git graph
- 简体中文语言包

4 语言环境配置-Python
官方渠道下载 https://www.python.org/downloads/

vscode插件安装：
- python语言包（包含pylance）

5 语言环境配置-Golang
官方渠道下载 https://go.dev/dl/ ，苹果芯片（m1/m2）选择 arm64 版本
设置goproxy
https://goproxy.cn/

vscode插件安装：
- golang语言包

打开vscode会提示安装 gopl，go-outline，点击安装即可

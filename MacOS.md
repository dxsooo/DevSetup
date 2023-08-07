# MacOS (基于MacOS 12)

## 基础配置
- 更新系统到最新
    - 【系统偏好设置】- 【软件更新】
- 设置触控板
    - 【系统偏好设置】- 【触控板】- 【光标与点按】，打开【轻点来点按】
- 配置网络
    - 右上角选 wifi
- 从dock移除不常用的应用
    - 双指点击图标，【选项】- 【从Dock移除】

## 终端（Terminal）配置
- 将终端从启动台的其他集合拉出到启动台，并再拉到dock中
- 将终端默认shell设置为 zsh
    - 点开【终端】- 工具栏【偏好设置】- 【通用】- 【shell的打开方式】 - 命令：/bin/zsh
- 安装 oh-my-zsh
    - 参考官网 https://ohmyz.sh/ ，选用 curl 方式（git会同时被下载安装）
    - 设置主题，修改 ~/.zshrc 文件中的 ZSH_THETE
        - 推荐：kphoen

## VPN配置
推荐使用 ClashX
- 从官方渠道下载：https://github.com/yichengchen/clashX/releases
- 配置：
    - 添加VPN配置文件：【配置】- 【托管配置】- 【管理】- 【添加】，url从VPN供应商获取
    - 增加规则：【配置】- 【更多设置】- 【忽略这些主机】，增加不需要走代理的域名
        - 譬如公司内网的一些域名
- 根据需要设置为系统代理
- 根据需要设置为开机启动

## VScode 配置
安装：

官方渠道下载：https://code.visualstudio.com/ ，下载后将app拉入【应用程序】
，打开程序并通过命令面板选择【在PATH中安装code命令】

插件安装：
- git graph
- 简体中文语言包
- GitLens （和git graph有功能重叠，树状显示效果git graph更佳，GitLens主要是inline git blame好用）
- Markdown Preview Mermaid Support

## 软件管理

一般都是遵循官网下载的方式进行软件安装，但是一些网站提供的下载方式是使用 homebrew，这时可以通过 homebrew 进行安装

homebrew 安装参考 https://brew.sh/

## 不同语言开发环境配置

- [Golang](./Golang.md)
- [Python](./Python.md)

## 通用开发

- [容器化](./Containerization.md)
- [数据库工具](./DatabaseTool.md)

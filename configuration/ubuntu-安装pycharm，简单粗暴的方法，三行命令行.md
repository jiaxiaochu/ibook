---
title: ubuntu-安装Pycharm，简单粗暴的方法，三行命令行
date: 2018-07-22 01:26:02
tags:  [环境配置,Python解释器的安装与配置,Pycharm]
categories: 『环境配置』- 工欲善其事，必先利其器
toc: true
<!-- thumbnail: https://ws1.sinaimg.cn/large/0065l1jqly1g57za9gz0hj30ze0m20yy.jpg -->
---

### 对于Ubuntu 16.10和Ubuntu 17.04，通过Ctrl + Alt + T打开终端，或通过从应用启动器搜索“terminal”，打开后，执行以下步骤：

1. .通过命令添加PPA存储库：
`sudo add-apt-repository ppa:mystic-mirage/pycharm`
***
<!-- more -->
2.如果您安装了以前的版本，请通过软件更新程序升级PyCharm。
##### 运行命令来检查更新并安装IDE（社区版本）
`sudo apt update`
`sudo apt install pycharm-professional`
***
##### 或运行命令来检查更新并安装IDE（社区版本）：
`sudo apt update`
`sudo apt install pycharm`
***
3.卸载PyCharm：
要卸载PyCharm Python IDE，只需运行命令：
专业版:  `sudo apt remove --autoremove pycharm pycharm-professional`  
社区版:   `sudo apt remove --autoremove pycharm pycharm-community`  

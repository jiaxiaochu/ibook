---
title: Ubuntu安装chrome浏览器和chromedriver
date: 2018-07-22 01:30:11
tags:  [环境配置,chromedriver,chrome]
categories: 『环境配置』- 工欲善其事，必先利其器
toc: true
<!-- thumbnail: https://ws1.sinaimg.cn/large/0065l1jqly1g57zrb1uecg30go07fnpg.gif -->
---

### 安装chrome步骤
***
###### 一. 下载chrome安装包
1. 使⽤ubuntu上的⽕狐浏览器打开如下地址：
`http://www.google.cn/intl/zhCN/chrome/browser/desktop/index.html`
<!-- more -->
2. 选择安装版本，接受并安装
a. 选择64bit.deb(适⽤于Deblan/Ubuntu)

3. 点击接受并安装后，选择保存到本地
a. ‘Save file’或者‘保存到本地’

4. 下载下来后，会保存在Dowdload⽂件中
cd ~/Dowdload 切换到下载⽂件⽬录中
ls 进⾏查看
***
### 二. 安装chrome浏览器
1. 打开终端，切换到root⽤户，进⼊下载⽂件夹
a. `cd ~/Dowdload`
b. `sudo dpkg -i google-chrome-stable_current_amd64.deb`

2. 初次安装如果出现 Errors where encountered while
processing:google-chrome-stable 这个错误，就需要安装googlechrome-stable
a. `apt-get install google-chrome-stable`

3. 如果安装了google-chrome-stable后，还报错，错误信息为： Unmet
dependencies. "Try apt-get -f install" with no packages (or
specify ....)
a. 这个时候按照提示执⾏
`apt-get -f install`

4. 如果中间提示"是否继续安装" 输⼊  `y`

v. 安装完毕后，重新执⾏第⼀步的命令
 `sudo dpkg -i google-chromestable_current_amd64.deb`

5. 如果此时没有报错就说明已经安装成功
***
### 三.安装chromedriver
1. 通过百度，搜索“淘宝NPM” 寻找chromedriver下载地址，点击进⼊

2. 通过百度，搜索“chrome和chromedriver的对照表”，选择⾃⼰的合适的chromedriver

3. 返回第⼀步打开的chromedriver版本⽹⻚，下载适合⾃⼰浏览器的chromedriver

4. 下载之后，在下载⽂件夹中找到，点击右键，选择解压到当前⽬录

5. **打开终端，将解压后的chromedriver执⾏程序，拷⻉到 /usr/bin ⽬录下**
 `cd~/Download`
 `sudo cp chromedriver /usr/bin`

6. 运⾏程序如果没有报错，说明选择的chromedriver的版本是正确的，如果还报错
说明版本没有选对，删除下载⽂件夹中的chromedriver⽂件和 /usr/bin 中的
chromedriver，重复上述步骤，选在适合⾃⼰浏览器的chromedriver下载安装

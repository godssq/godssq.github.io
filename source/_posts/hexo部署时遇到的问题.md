---
title: hexo部署时遇到的问题
date: 2020-12-12 23:45:27
tags:
---
hexo d 时出现以下乱码：
fatal: unable to access 'https://github.com/Qy709/Qy709.github.io/ ': Failed to connect to localhost port 8080: Connection refused
.......
解决方法：
输入以下代码即可：
git config --global --unset http.proxy
git config --global --unset https.proxy



hexo d 时需要输入登录账号密码：
修改repo
改为https//(your name):(your password)@github,com/(your name)/(your name).github.io.git
即可
---
title: mac ~/.bash_profile配置重启后不生效的解决方法
tags:
- linux
- macOS
categories:
- hexo
---

zsh加载的是 ~/.zshrc文件，而 ‘.zshrc’ 文件中并没有定义任务环境变量。

解决办法

在~/.zshrc文件最后，增加一行： 
``` bash
$ source ~/.bash_profile
```
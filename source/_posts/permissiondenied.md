---
title: macOS下 npm install 报错 "permission denied"
tags:
- nodejs
- npm
- macOS
categories:
- hexo
---

``` bash
npm ERR! Error: EACCES: permission denied, mkdir '/Users/xxxxx/.npm/_cacache/index-v5/ad/a1'
npm ERR!  { [Error: EACCES: permission denied, mkdir '/Users/
xxxxx/.npm/_cacache/index-v5/ad/a1']
npm ERR!   cause:
npm ERR!    { Error: EACCES: permission denied, mkdir '/Users/x x x xx/.npm/_cacache/index-v5/ad/a1'
npm ERR!      errno: -13,
npm ERR!      code: 'EACCES',
npm ERR!      syscall: 'mkdir',
npm ERR!      path: '/Users/xxxxx/.npm/_cacache/index-v5/ad/a1' },
npm ERR!   isOperational: true,

```
权限上出了问题，解决方式：

``` bash

$ sudo chown -R $USER:$GROUP ~/.npm
$ sudo chown -R $USER:$GROUP ~/.config

```
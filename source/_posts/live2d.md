---
title: 为你的博客添加live2d模型
tags:
- live2d
- hexo
categories:
- hexo
---

首先安装hexo-helper-live2d包： 
``` bash
$ npm install --save hexo-helper-live2d
```
然后在根目录修改_config.yml 配置
``` bash
live2d:
  enable: true
  scriptFrom: local
  pluginRootPath: live2dw/
  pluginJsPath: lib/
  pluginModelPath: assets/
  tagMode: false
  debug: false
  model:
    use: live2d-widget-model-hijiki  
  display:
    position: right
    width: 150
    height: 300
  mobile:
    show: true
```

以下是所有主题，然后 npm install {packagename}  你要想的主题：
附上主题来源 ：(https://github.com/xiazeyu/live2d-widget-models/blob/master/README.md)

``` bash
live2d-widget-model-chitose
live2d-widget-model-epsilon2_1
live2d-widget-model-gf
live2d-widget-model-haru/01 (use npm install --save live2d-widget-model-haru)
live2d-widget-model-haru/02 (use npm install --save live2d-widget-model-haru)
live2d-widget-model-haruto
live2d-widget-model-hibiki
live2d-widget-model-hijiki
live2d-widget-model-izumi
live2d-widget-model-koharu
live2d-widget-model-miku
live2d-widget-model-ni-j
live2d-widget-model-nico
live2d-widget-model-nietzsche
live2d-widget-model-nipsilon
live2d-widget-model-nito
live2d-widget-model-shizuku
live2d-widget-model-tororo
live2d-widget-model-tsumiki
live2d-widget-model-unitychan
live2d-widget-model-wanko
live2d-widget-model-z16
```

接着把上面关于live2d的use 的配置改为你上面install好的主题名，接着hexo server 看看是不是一个可爱的live2d模型出现在你的博客右下角了呢！

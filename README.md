# IE-Out 浏览器升级引导组件

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

当检测到用户使用旧版IE浏览器访问时，自动跳转到浏览器升级引导页的轻量级解决方案。

> 灵感源自 [旧版 Internet Explorer 淘汰行动](https://support.dmeng.net/kill-old-versions-of-ie.html) 。但原项目已经很久没有更新，故经修改，分享给大家！

别忘记点个 Star！

## 🚀 功能特性
- 精准识别 IE 8-11 浏览器版本
- 智能跳转至升级引导页
- 支持主流现代浏览器白名单
- 轻量级无依赖实现

<!-- - 自动携带来源页面URL参数 --> 

## 🛠 快速集成

### 1. 引入检测代码
您需要在需要启用 ie-out 的网页添加以下代码：
> 注意： window.location.href="<这里修改您的跳转链接>"

```
/* IE-Out Detection */
<script>window.MSInputMethodContext&&document.documentMode&&(window.location.href="/lib/upgrade-your-browser/index.html?referrer="+encodeURIComponent(window.location.href));</script>
``` 

### 2. 部署引导页面
同时将 upgrade-your-browser 中的文件复制到您的服务器：

```
upgrade-your-browser/
├── assets/
│   ├── css/
│   │   ├── support.style.min.css
│   │   └── switch_mode.style.min.css
│   ├── images/
│   │   ├── chrome.png
│   │   ├── edge.png
│   │   ├── ee360.png
│   │   ├── example.png
│   │   ├── firefox.png
│   │   ├── qqbrowser.png
│   │   └── safari.png
│   └── js/
│       ├── er3eport.min.js
│       └── main.min.js
├── guides/
│   ├── end-of-ie-support/
│   │   └── index.html
│   └── switch-mode/
│       └── index.html
├── media.mp4
├── favicon.ico
└── index.html
```

建议将目录放置于网站根目录下的 /lib/upgrade-your-browser/。

# 🎨界面预览

<div align="center">

  ![请升级您的浏览器.png](https://smms.app/image/CTpaWgrnGvmAb5H)

  **图1 浏览器升级主引导页**

</div>
<div align="center">

  ![如何切换到极速模式.png](https://smms.app/image/t72C1MoAhpI84ei)

  **图2 浏览器极速模式切换指引**

</div>
<div align="center">

  ![Internet Explorer 11 桌面应用停用常见问题解答.png](https://smms.app/image/PU6QjzAcbytWhMk)

  **图3 IE停用说明**

</div>

# License
MIT

# 简介
将 ie-out 移植到您的网站，用户使用 IE 访问网站时自动跳转到提醒升级浏览器的页面。
灵感来源于 旧版 Internet Explorer 淘汰行动(https://support.dmeng.net/kill-old-versions-of-ie.html) 。但原项目已经很久没有更新，故经修改，分享给大家！

# 需要添加的代码
您需要在需要启用 ie-out 的网页添加以下代码：
> 注意： window.location.href="<这里修改您的跳转链接>"

```
/* IE-Out */
<script>window.MSInputMethodContext&&document.documentMode&&(window.location.href="/lib/upgrade-your-browser/index.html?referrer="+encodeURIComponent(window.location.href));</script>
``` 

同时将 upgrade-your-browser 中的文件复制到您的网站目录。

# 网页展示
![请升级您的浏览器 - 六月的风.png](https://s2.loli.net/2023/02/12/rV9t6TaMnpSWRJK.png)
![如何切换到极速模式.png](https://s2.loli.net/2023/02/12/WLYR9SyFIhmswfl.png)
![Internet Explorer 11 桌面应用停用常见问题解答.png](https://s2.loli.net/2023/02/12/GyiKeaghuWNj1O9.png)

# License
MIT

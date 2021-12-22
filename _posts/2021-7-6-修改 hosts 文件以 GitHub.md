---
layout:     post
title:      修改 hosts 文件以破壁
subtitle:   Github
date:       2021-7-6
author:     许江一墨
header-img: img/the-first.png
catalog:   true
tags:
    - 杂谈
---

我们可以通过修改 hosts 文件内容使得被墙的 GitHub 可访问。

```
## GitHub Start

192.30.253.112 http://github.com

192.30.253.113 http://github.com

151.101.184.133 http://assets-cdn.github.com

151.101.185.194 http://github.global.ssl.fastly.net

192.30.253.112 http://github.com

192.30.253.113 http://github.com

192.30.253.118 http://gist.github.com

151.101.185.194 http://github.global.ssl.fastly.net

151.101.129.194 http://github.global.ssl.fastly.net

151.101.65.194 http://github.global.ssl.fastly.net

151.101.1.194 http://github.global.ssl.fastly.net

151.101.193.194 http://github.global.ssl.fastly.net

151.101.77.194 http://github.global.ssl.fastly.net

151.101.229.194 http://github.global.ssl.fastly.net

151.101.113.194 http://github.global.ssl.fastly.net

151.101.196.133 http://assets-cdn.github.com

151.101.24.133 http://assets-cdn.github.com

185.199.111.153 http://assets-cdn.github.com

185.199.110.153 http://assets-cdn.github.com

185.199.108.153 http://assets-cdn.github.com

185.199.109.153 http://assets-cdn.github.com

151.101.112.133 http://assets-cdn.github.com

151.101.112.133 http://avatars0.githubusercontent.com

151.101.112.133 http://avatars1.githubusercontent.com

151.101.184.133 http://avatars2.githubusercontent.com

151.101.12.133 http://avatars3.githubusercontent.com

151.101.12.133 http://avatars4.githubusercontent.com

151.101.184.133 http://avatars5.githubusercontent.com

151.101.184.133 http://avatars6.githubusercontent.com

151.101.184.133 http://avatars7.githubusercontent.com

151.101.12.133 http://avatars8.githubusercontent.com

151.101.184.133 http://raw.githubusercontent.com

151.101.112.133 http://gist.githubusercontent.com

151.101.184.133 http://cloud.githubusercontent.com

151.101.112.133 http://camo.githubusercontent.com

52.216.227.168 http://github-cloud.s3.amazonaws.com

192.30.253.112 http://github.com

185.199.108.153 http://assets-cdn.github.com

151.101.185.194 http://github.global.ssl.fastly.net

140.82.113.10 http://codeload.github.com

# 下载慢问题
219.76.4.4 http://github-cloud.s3.amazonaws.com

## GitHub End
```

将以上代码复制粘贴到hosts文件末尾即可，记得保存。

修改hosts前记得先修改hosts的文件属性并使其可以访问。

------

修改完成后，我们需要刷新配置使得修改生效。

这里介绍两种方法：

1. 重启电脑（简单粗暴）。
2. 快捷键 `win + R` 键入 `cmd` ， 在弹出的窗口中输入 `ipconfig /flushdns` 等待即可。

以上便是修改 hosts 文件 访问 GitHub 的方法。
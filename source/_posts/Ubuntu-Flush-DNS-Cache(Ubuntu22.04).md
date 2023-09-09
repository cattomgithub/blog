---
title: Ubuntu 刷新 DNS 缓存 (Ubuntu 22.04)
date: 2023-09-10 02:35:01
tags: [Ubuntu,DNS,Linux]
excerpt: "本文介绍了 Ubuntu 22.04 刷新 DNS 缓存的方法。"
---
## 查看 DNS 缓存情况

```sh
sudo resolvectl statistics
```

## 刷新 DNS 缓存

```sh
sudo resolvectl flush-caches
```

## 另：刷新 Chrome 中的 DNS 缓存

在地址栏中输入 `chrome://net-internals/#dns` 回车打开

然后点击 **Clear host cache**
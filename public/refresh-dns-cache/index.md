# [Ubuntu 20.04]刷新 DNS 缓存

## 查看 DNS 缓存情况

```bash
sudo systemd-resolve --statistics
```

## 刷新 DNS 缓存

```bash
sudo systemd-resolve --flush-caches
```

## 刷新 Chrome 中的 DNS 缓存

在地址栏中输入 `chrome://net-internals/#dns`

回车打开

然后点击 **Clear host cache**

---
title: "[Ubuntu 20.04]Realtek ALC294无声音解决"
description: "Realtek ALC294 声卡在 Ubuntu 20.04 下外放/耳机无声音的解决方案。"
date: 2021-08-04
slug: fix-no-sound-realtek-alc294
categories:
  - tech
tags:
  - 教程
summary: Realtek ALC294 声卡在 Ubuntu 20.04 下外放/耳机无声音的解决方案。
featuredImage: "https://static.cattom.site/image/ubuntu20.04.png?x-oss-process=style/webp"
--- 
## 环境
* ASUS FL8000U
* Ubuntu 20.04

## 问题
**Realtek ALC294** 声卡在 **Ubuntu 20.04** 下外放/耳机无声音

估计这个问题应该只要是 ASUS 都可能会遇到，不论笔记本还是主板...

## 解决
1. 修改 `/etc/modprobe.d/alsa-base.conf`
2. 在文件的最后添加 `options snd-hda-intel model=asus-zenbook`
3. 保存文件后，重启电脑

## 附：查看你使用的声卡型号
一般声卡都是在 **device 0**
```bash
aplay -l

**** PLAYBACK 硬體裝置清單 ****
card 0: PCH [HDA Intel PCH], device 0: ALC294 Analog [ALC294 Analog]
  子设备: 1/1
  子设备 #0: subdevice #0

...
```
## 参考
[Ask Ubuntu - No sound ALC294 Asus ROG Strix 512 Ubuntu 20.04.01](https://askubuntu.com/questions/1276428/no-sound-alc294-asus-rog-strix-512-ubuntu-20-04-01/)
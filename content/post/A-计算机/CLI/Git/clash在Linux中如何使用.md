---
title: clash在Linux中如何使用
description: 简单表述一下clash在Linux系统中如何使用
date: 2024-01-13T00:09:24+08:00
license: 
tags:
  - linux
categories:
  - 计算机
---
## 值得细讲的点

### Linux的Clash，因为在github上，clash删库跑路了，所以现存的clash压缩包

```shell
wget https://github.com/Dreamacro/clash/releases/download/v1.14.0/clash-linux-amd64-v1.14.0.gz
```

建议自己也存一份

`curl https://glados.rocks/tools/clash-linux.zip -o clash.zip`

### 解压(unzip)

### 上传配置文件(就是机场订阅链接下载下来的哪个yaml文件)

### 启动

`./clash-linux-amd64-v1.10.0 -f glados.yaml -d .`

### 设置环境变量

```sh
export https_proxy=http://127.0.0.1:7890 
export http_proxy=http://127.0.0.1:7890
export all_proxy=socks5://127.0.0.1:7890
```

## 参考

[在 Linux 中使用 Clash | CodeSwift (iswiftai.com)](https://blog.iswiftai.com/posts/clash-linux/)

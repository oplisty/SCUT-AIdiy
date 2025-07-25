---
description: 众所周知我们训模型需要用到大量的GPU所以我们一般都会租用显卡集群，实验室也一般有自己的显卡集群
---

# 服务器连接

一般服务器信息包含

```
4090服务器
IP：
端口：
用户名：
密码：
```

**终端SSH连接**

指令为

```
ssh 用户名@ip地址 -p 端口号
```

接着输入密码即可

**免密登录**

我们如果每次登录服务器都要输入密码对于我这种懒人肯定不太友好那可不可以免密呢？当然可以首先我们需要生成密钥对

```
ssh-keygen -t rsa -b 4096
```

接着呢把密钥对上传到服务器

```
ssh-copy-id -p 端口号 用户名@ip地址
```

然后指令和ssh一样就可以免密登录了

**Vscode连接**

* 拓展搜 SSH Remote

<figure><img src="../.gitbook/assets/image-20250709223539864.png" alt=""><figcaption></figcaption></figure>

* 添加服务器(右上角加号)

<figure><img src="../.gitbook/assets/image-20250709224003747 (1).png" alt=""><figcaption></figcaption></figure>

* 然后输入ssh指令就会自动给你配置到setting.json中就能连接成功了

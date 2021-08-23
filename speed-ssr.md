# Linux一键安装常见/最新内核脚本 锐速/BBRPLUS/BBR2


## 卸载内核

```
wget -N --no-check-certificate "https://github.000060000.xyz/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
或

wget -O tcp.sh "https://git.io/coolspeeda" && chmod +x tcp.sh && ./tcp.sh
```

## 不卸载内核

```
wget -N --no-check-certificate "https://github.000060000.xyz/tcpx.sh" && chmod +x tcpx.sh && ./tcpx.sh
或

wget -O tcpx.sh "https://git.io/JYxKU" && chmod +x tcpx.sh && ./tcpx.sh
```

## 锐速/bbr/bbrplus 对应的版本：

```
跟随github地址为https://github.com/ylx2016/kernel/releases
不卸载版本22优化项默认开启tcp fast open，卸载默认关闭
```



| 加速方式                        | 系统             | 版本                 |
| ------------------------------- | ---------------- | -------------------- |
| BBR                             | centos7          | 跟随github           |
|                                 | debian/ubuntu    | 跟随github 支持ARM64 |
| BBRPLUS（）                     | centos7          | 4.14.129             |
|                                 | debian/ubuntu    | 4.14.129             |
| BBRPLUS新版号 仅限Cloud VMs     | centos7          | 跟随github           |
|                                 | debian/ubuntu    | 跟随github           |
| XANMOD – 当前为最新LTS内核<br/>BBR2 | centos7、centos8 | 跟随github           |
|                                 | debian/ubuntu    | 跟随官方             |
| 锐速 |  | 不统计版本太杂 |

> **安装中提示Abort kernel removal?选择No**

```

https://github.com/ylx2016/Linux-NetSpeed

https://github.com/ylx2016/kernel/releases

# 查看真实队列？
tc -s qdisc show


```


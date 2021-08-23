<h1>自建Shadowsocks服务器简明教程</h1>

**自建Shadowsocks教程很简单，整个教程分简单几步**：

购买香港或者国外服务器、一键加速VPS服务器、安装Shadowsocks服务端

***

**【前言】**

**Shadowsocks的优势**

Shadowsocks（简称SS） 和 ShadowsocksR（简称SSR）听起来都挺耳熟，今天先不说二者的详细区别，只说一件事：在自建翻墙服务器之前，笔者曾使用了一段时间 [搬瓦工的Just My Socks翻墙服务](https://github.com/killgcd/justmysocks/blob/master/README.md) ,发现他家不支持SSR，于是就去问了一下为啥不支持SSR呢，很快就得到了回复，回复的原文如下：

>We do not currently support Shadowsocks-R. Our main concern about Shadowsocks-R is that its server code hasn't seen any major updates since 2015 -- looks like it was abandoned by developer(s).

>Additionally, according to our observations, it is more easily detected by government blocking solutions (especially lately in 2019).

>We recommend using vanilla (original) Shadowsocks client applications as they are actively maintained.

简单翻译一下，大意是说：

>我们（）目前不支持Shadowsocks-R。我们对Shadowsocks-R的主要担心是，自2015年以来，其服务器代码未见任何重大更新-似乎已被开发人员放弃。

>此外，根据我们的观察，政府阻止解决方案（尤其是2019年末）更容易检测到它。

>我们建议使用 Vanilla (original) Shadowsocks 客户端应用程序，因为它们会得到积极维护。

简单想想，的确在理，为了对抗不断升级的网络封锁，软件能够持续的更新和维护显然是一个最大的优势了。

***

## **第一步：购买服务器**

百度

***

### **第二步：SSH连接服务器**

百度

***

### 第三步：BBR 一键加速

[点我查看](./speed-ssr.md)



***

### **第四步：安装Shadowsocks服务端**

```
wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
```




***

### **第五步：客户端配置**

#### Shadowsocks/SS客户端

| **SS Windows客户端** | [4.1.7.1修复版](https://tlanyan.pp.ua/download.php?filename=/ss/windows/Shadowsocks-win-4.1.7.1-tlanyan.zip)  \|  [官方4.4.0.0版](https://tlanyan.pp.ua/download.php?filename=/ss/windows/Shadowsocks-4.4.0.185.zip) | [官网下载](https://github.com/shadowsocks/shadowsocks-windows/releases) | [ss windows客户端配置教程](https://tlanyan.pp.ua/go.php?key=ss-win-config) |
| -------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **SS 安卓客户端**    | [Shadowsocks 5.2.5.apk](https://tlanyan.pp.ua/download.php?filename=/ss/android/shadowsocks--universal-5.2.5.apk) | [官网下载](https://github.com/shadowsocks/shadowsocks-android/releases) | [ss安卓客户端配置教程](https://tlanyan.pp.ua/go.php?key=ss-an-config) |
| **SS MAC客户端**     | [ShadowsocksX-NG 1.9.4.zip](https://tlanyan.pp.ua/download.php?filename=/ss/macos/ShadowsocksX-NG.1.9.4.zip) | [官网下载](https://github.com/shadowsocks/ShadowsocksX-NG/releases) | [ss mac客户端配置教程](https://tlanyan.pp.ua/go.php?key=ss-mac-config) |

#### Shadowsocks/SSR客户端

| **SSR Windows客户端**    | [ShadowsocksR 4.9.2修复版](https://tlanyan.pp.ua/download.php?filename=/ssr/windows/ShadowsocksR-win-4.9.2-tlanyan.zip) | [官网下载](https://github.com/shadowsocksrr/shadowsocksr-csharp/releases) | [SSR Windows客户端配置教程](https://tlanyan.pp.ua/go.php?key=ssr-win-config) |
| ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
|                          | [ShadowsocksR 4.9.2官方版](https://tlanyan.pp.ua/download.php?filename=/ssr/windows/ShadowsocksR-win-4.9.2.zip) | [官网下载](https://github.com/shadowsocksrr/shadowsocksr-csharp/releases) |                                                              |
|                          | [Netch-v1.8.7.7z](https://tlanyan.pp.ua/download.php?filename=/v2/windows/Netch-v1.8.7.7z) | [官网下载](https://github.com/NetchX/Netch/releases)         |                                                              |
| **SSR 安卓客户端**       | [ShadowsocksR 3.5.4.apk](https://tlanyan.pp.ua/download.php?filename=/ssr/android/shadowsocksr-android-3.5.4.apk) | [官网下载](https://github.com/shadowsocksrr/shadowsocksr-android/releases) | [SSR安卓客户端配置教程](https://tlanyan.pp.ua/go.php?key=ssr-an-config) |
|                          | [ssrray-v3.8.11.apk](https://tlanyan.pp.ua/download.php?filename=/v2/android/ssrray-v3.8.11.apk) | [官网下载](https://github.com/xxf098/shadowsocksr-v2ray-trojan-android/releases) |                                                              |
| **SSR MAC客户端**        | [ShadowsocksX-NG-R8.dmg](https://tlanyan.pp.ua/download.php?filename=/ssr/macos/ShadowsocksX-NG-R8.dmg) | [官网下载](https://github.com/qinyuhang/ShadowsocksX-NG-R/releases) | [SSR MAC客户端配置教程](https://tlanyan.pp.ua/go.php?key=ssr-mac-config) |
| **SS/SSR 免费iOS客户端** | Mume（图标是一朵梅花，有红梅/黑梅两个版本，黑梅免费且内置免费节点） Potatso Lite NetShuttle(网际飞梭) Sockswitch（没有中文界面） ConnectSPro ShadowLink Brook（只支持aes-256-cfb算法） Surge（高级工具，不适合新手） shadowrock |                                                              | 个人推荐使用Mume和Potatso lite，简洁好用                     |
| **SS/SSR 收费iOS客户端** | Shadowrocket（俗称小火箭，注意不是shadowrocket VPN） [配置教程](https://v2xtls.org/小火箭shadowrocket配置ss-ssr教程/) pepi Potasto 2 Wingy surge pro |                                                              | 个人推荐Shadowrocket和pepi                                   |

> 注意：有些shadowsocks客户端已经下架，但app store中存在同名的应用，请注意区分，例如Waterdrop、MUME。
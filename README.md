

# Action Openwrt 云自动编译
⏰ **每天自动拉取最新源码自动编译**

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<br />

<p align="center">
  <a href="https://github.com/jlqwer/openwrt-rpi4">
    <img src="https://cdn.jsdelivr.net/gh/bigbugcc/Resource@master/github/openwrts/action1.jpg" alt="Logo" width="500" />
  </a>

  <h3 align="center">Openwrt/LEDE 云编译</h3>
  <p align="center">
    👉 每天定时自动拉取Openwrt最新源码编译，自动发布到 [<a herf="https://github.com/jlqwer/openwrt-rpi4/releases"> Releases </a>]👈
    <br />
    <a href="https://github.com/jlqwer/openwrt-rpi4"><strong>探索本项目的文档 »</strong></a>
    <br />
    <br />
    <a href="https://github.com/jlqwer/openwrt-rpi4/releases">下载地址</a>
    ·
    <a href="https://github.com/jlqwer/openwrt-rpi4/actions">Action</a>
    ·
    <a href="https://github.com/jlqwer/openwrt-rpi4/issues">提出新特性</a>
  </p>

</p>

## 目录

- [支持的设备](#支持的设备)  

- [Action Openwrt 云自动编译](#action-openwrt-云自动编译)
  - [目录](#目录)
  - [支持的设备](#支持的设备)
    - [🎯固件默认设置](#固件默认设置)
  - [固件特性](#固件特性)
  - [自带插件](#自带插件)
  - [文件目录说明](#文件目录说明)
  - [定制固件](#定制固件)
    - [注意事项：](#注意事项)
  - [固件预览](#固件预览)
  - [版权说明](#版权说明)
  - [项目支持](#项目支持)

<br>


## 支持的设备
|           支持的设备        |         固类别         |        Action         |            状态          |              下载页          |
| :------------------------: | :---------------------: | :-------------------: | :-------------------: | :--------------------------: |
|             树莓派 4B             |  [LEDE](https://github.com/coolsnowwolf/lede) | [🍕](https://github.com/jlqwer/openwrt-rpi4/actions/workflows/RaspberryPi4.yml) | ![RaspberryPi4](https://github.com/jlqwer/openwrt-rpi4/actions/workflows/RaspberryPi4.yml/badge.svg) |  [✔](https://github.com/jlqwer/openwrt-rpi4/releases) |

<br>

### 🎯固件默认设置   
- 路由器地址: `192.168.7.1`   
- 默认用户名: `root`   
- 默认密码  : `password`

<br>

## 固件特性
✨ 自带常用的插件   
✨ 集成所有openwrt的USB驱动   
✨ 集成Python3.x(带pip)环境   
✨ 集成Docker-CE   
✨ 集成Node.js(14.xLTS 带npm、yarn)   
✨ 全新的 [Them](https://github.com/jerrykuku/luci-theme-argon)  
✨ x86_64 vmdk固件集成vm-tools   

<br>

## 自带插件
🍕 默认插件
- PassWall / SSR Plus
- AdGuard Home
- Mentohust
- luci-app-vssr   
- luci-app-unblockmusic
- luci-app-ddns
- luci-app-onliner
- luci-app-ttyd
- luci-app-turboacc
- luci-app-upnp
- luci-usb-printer
- luci-app-nps
- luci-app-syncdial (多播插件)
- luci-app-turboacc
- luci-app-kms  
- luci-app-docker   
- luci-app-serverchan   
- luci-app-control-timewol (定时wol唤醒)   
- luci-app-aliyundrive-webdav (阿里云盘)  
- luci-app-filebrowser   
- luci-app-nfs   
......

<br>

## 文件目录说明
eg:

```
filetree 
├── .github/workflows
│  ├── RaspberryPi4.yml
│  ├── update-checker.yml
├── /configs/ (配置文件目录)
│  ├── RPi4.config
├── configure.sh (固件参数修改)
├── package.sh (luci-app)
```
<br>

## 定制固件 
1. Fork 此项目
2. 按需修改 ```configure.sh``` 和 ```package.sh``` 文件
3. 上传你自己的 ```xx.config``` 配置文件到configs目录 
4. 添加或修改自己的``````xx.yml``````文件 
5. 最后根据个人喜好修改 ```update-checker.yml``` 需自行添加 ```Actions secrets``` (触发自动编译)

### 注意事项：
📌 修改默认系统参数 👉 ```configure.sh```   
📌 添加其它Luci插件 👉 ```package.sh```  
📌 其它机型添加 👉 ```.github/workflows``` 目录下并上传 ```.config```文件到 ```/configs/```目录下

<br>

## 固件预览
**主界面：**
![主界面](https://cdn.jsdelivr.net/gh/bigbugcc/Resource@latest/github/openwrts/openwrt.png)

**服务/插件：**
![服务/插件](https://cdn.jsdelivr.net/gh/bigbugcc/Resource@latest/github/openwrts/service.png)

**网络：**
![网络](https://cdn.jsdelivr.net/gh/bigbugcc/Resource@latest/github/openwrts/network.png)

## 版权说明

该项目签署了MIT 授权许可，详情请参阅 [LICENSE](https://github.com/jlqwer/openwrt-rpi4/LICENSE)

<br>




## 项目支持
- [P3TERX/Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [luci-theme-argon](https://github.com/jerrykuku/luci-theme-argon)

<!-- links -->
[your-project-path]:https://github.com/jlqwer/openwrt-rpi4/
[contributors-shield]: https://img.shields.io/github/contributors/jlqwer/openwrt-rpi4?style=flat-square
[contributors-url]: https://github.com/jlqwer/openwrt-rpi4/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/jlqwer/openwrt-rpi4?style=flat-square
[forks-url]: https://github.com/jlqwer/openwrt-rpi4/network/members
[stars-shield]: https://img.shields.io/github/stars/jlqwer/openwrt-rpi4?style=flat-square
[stars-url]: https://github.com/jlqwer/openwrt-rpi4/stargazers
[issues-shield]: https://img.shields.io/github/issues/jlqwer/openwrt-rpi4?style=flat-square
[issues-url]: https://img.shields.io/github/issues/jlqwer/openwrt-rpi4
[license-shield]: https://img.shields.io/github/license/jlqwer/openwrt-rpi4?style=flat-square
[license-url]: https://github.com/jlqwer/openwrt-rpi4/blob/main/LICENSE
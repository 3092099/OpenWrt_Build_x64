<div align="center">
<img width="768" src="https://github.com/3092099/OpenWrt_Build_x64/blob/main/personal/logo.png"/>
<h1>OpenWrt_Build_x64</h1>
</div>

## 当前编译状态：
|    序号    |     架构名称    |    编译状态    |    固件下载    |
| :-----------------: | :-------------: |:-----------------: | :-----------------: |
| 1 |1806_x64_全功能版|<a href="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_all.yml"><img src="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_all.yml/badge.svg?style=flat" /></a>    |[下载地址](https://github.com/3092099/OpenWrt_Build_x64/releases/tag/OpenWrt_1806_x64_all)    |
| 2 |1806_x64_主路由版|<a href="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_wjq.yml"><img src="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_wjq.yml/badge.svg?style=flat" /></a>    |[下载地址](https://github.com/3092099/OpenWrt_Build_x64/releases/tag/OpenWrt_1806_x64_wjq)    |
| 3 |1806_x64_旁路由版|<a href="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_gxnas.yml"><img src="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_gxnas.yml/badge.svg?style=flat" /></a>    |[下载地址](https://github.com/3092099/OpenWrt_Build_x64/releases/tag/OpenWrt_1806_x64_gxnas)    |
| 4 |1806_x64_精简版|<a href="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_soot.yml"><img src="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_soot.yml/badge.svg?style=flat" /></a>    |[下载地址](https://github.com/3092099/OpenWrt_Build_x64/releases/tag/OpenWrt_1806_x64_soot)    |
| 5 |1806_x64_测试版|<a href="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_test.yml"><img src="https://github.com/3092099/OpenWrt_Build_x64/actions/workflows/OpenWrt_Build_1806_x64_test.yml/badge.svg?style=flat" /></a>    |[下载地址](https://github.com/3092099/OpenWrt_Build_x64/releases/tag/OpenWrt_1806_x64_test)    |

</br>

## 项目说明 [![](https://github.com/3092099/OpenWrt_Build_x64/blob/main/personal/describes.svg)](#项目说明-)
- 固件来源：[![Lean](https://img.shields.io/badge/Lede-Lean-red.svg?style=flat&logo=appveyor)](https://github.com/coolsnowwolf/lede) 
- 项目使用 Github Actions 拉取 [Lean](https://github.com/coolsnowwolf/lede) 的 `Openwrt` 源码仓库进行云编译
- 🔴x86[全功能版] 固件默认的IP地址：`192.168.18.1` 默认密码：`无密码`
- 🔴x86[主路由版] 固件默认 IP 地址：`192.168.18.1` 默认密码：`无密码`
- 🔴x86[旁路由版] 固件默认 IP 地址：`192.168.1.11` 默认密码：`无密码`
- 🔴x86[精简版] 固件默认 IP 地址：`192.168.1.11` 默认密码：`无密码`
-  本库编译的x86固件为squashfs格式；
-  ext4 与squashfs 格式的区别： ext4 格式的rootfs 可以扩展磁盘空间大小，而squashfs 不能。 squashfs 格式的rootfs 可以使用重置功能（恢复出厂设置），而ext4 不能。
-  默认的固件容量：Kernel=32M、rootfs=968M，请确保你的OpenWrt硬盘空间至少要有1G以上；
-  升级方法：下载好对应版本的.img.gz文件到电脑上，不需要解压，然后在你的OpenWrt菜单“系统-备份/升级”直接选择下载好的.img.gz文件上传，刷写固件；
- 🛑******建议全新刷机可获得最佳的体验******

## 插件预览 [![](https://github.com/3092099/OpenWrt_Build_x64/blob/main/personal/preview.svg)](#插件预览-)
<details>
<summary><b>&nbsp; 插件预览</b></summary>
<br/>
<details>
<summary><b>├── 状态</b></summary>
　├── 概况<br/>
　├── 防火墙<br/>
　├── 路由表<br/>
　├── 系统日志<br/>
　├── 内核日志<br/>
　├── 系统进程<br/>
　├── 实时信息<br/>
　├── 实时监控<br/>
　├── WireGuard状态<br/>
　├── 负载均衡<br/>
　└── 释放内存
</details>
<details>
<summary><b>├── 系统</b></summary>
　├── 系统<br/>
　├── Web管理<br/>
　├── 管理权<br/>
　├── 软件包<br/>
　├── TTYD 终端<br/>
　├── 启动项<br/>
　├── 计划任务<br/>
　├── 挂载点<br/>
　├── 磁盘管理<br/>
　├── 备份/升级<br/>
　├── 定时设置<br/>
　├── 文件传输<br/>
　├── Argon 主题设置<br/>
　├── Design 主题设置<br/>
　├── 重启<br/>
　└── 关机
</details>
<details>
<summary><b>├── 服务</b></summary>
　├── PassWall<br/>
　├── PassWall2  (arm)<br/>
　├── Hello World<br/>
　├── AdGuard Home<br/>
　├── ShadowSocksR Plus+<br/>
　├── DDNSTO 远程控制<br/>
　├── 应用过滤<br/>
　├── 网站域名黑白名单配置<br/>
　├── 全能推送<br/>
　├── 上网时间控制<br/>
　├── OpenClash<br/>
　├── Lucky<br/>
　├── 动态 DNS<br/>
　├── SmartDNS<br/>
　├── MosDNS<br/>
　├── 网络唤醒<br/>
　├── Frps<br/>
　├── UPnP<br/>
　├── Frp 内网穿透<br/>
　├── KMS 服务器<br/>
　└── Nps 内网穿透
</details>
<details>
<summary><b>├── Docker  (arm)</b></summary>
　├── 概览<br/>
　├── 容器<br/>
　├── 镜像<br/>
　├── 网络<br/>
　├── 存储卷<br/>
　├── 事件<br/>
　└── 设置
</details>
<details>
<summary><b>├── 网络存储</b></summary>
　├── 文件浏览器<br/>
　├── NFS 管理<br/>
　├── Alist 文件列表<br/>
　├── USB 打印服务器<br/>
　├── 硬盘休眠<br/>
　├── 打印服务器<br/>
　├── 网络共享<br/>
　├── Aria2 配置<br/>
　└── FTP 服务器
</details>
<details>
<summary><b>├── VPN</b></summary>
　├── V2ray 服务器<br/>
　├── N2N VPN<br/>
　├── SoftEther VPN 服务器<br/>
　├── OpenVPN 服务器<br/>
　├── IPSec VPN 服务器<br/>
　├── PPTP VPN 服务器<br/>
　└── ZeroTier
</details>
<details>
<summary><b>├── 网络</b></summary>
　├── 接口<br/>
　├── DHCP/DNS<br/>
　├── 主机名<br/>
　├── IP/MAC 绑定<br/>
　├── 静态路由<br/>
　├── 防火墙<br/>
　├── 诊断<br/>
　├── IP限速<br/>
　├── Socat<br/>
　├── Turbo ACC 网络加速<br/>
　├── 多线多拨<br/>
　└── 负载均衡
</details>
<details>
<summary><b>├── 带宽监控</b></summary>
　├── 显示<br/>
　├── 配置<br/>
　├── 备份<br/>
　└── 实时流量监测
</details>
　└── <b>退出</b>
</details>

<a href="#readme">
<img src="https://github.com/3092099/OpenWrt_Build_x64/blob/main/personal/return.svg" title="返回顶部" align="right"/>
</a>

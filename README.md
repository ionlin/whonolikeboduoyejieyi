# OpenWrt中国大陆              

![1](https://user-images.githubusercontent.com/73426989/121067818-1a316f00-c7fe-11eb-9978-4fe568193fd4.png)           

## OpenWrt_Pro专区    

支持：x64 * r2s * r4s * r2c         
  
* [OpenWrt_Pro](https://t.me/openwrt_p)

## OpenWrt_mini专区             

支持：x64           

* [OpenWrt_mini](https://t.me/openwrt_m)         

## OpenWrt_Air专区        

支持：acrh17 * 

* [OpenWrt_Air](https://t.me/openwrt_a)             

## 配套工具区    

* [cn_windows_10_pro_lite_21h1_x64](https://h8cs-my.sharepoint.com/:u:/g/personal/od577_365a1_me/EQP8VVFniwFDuc8RJyIwIIIBYDb6DgYcEj4oUTYpus_dng?e=hLypsb)             
* [PVE 7.0-9、10、11、13显示CPU主频、CPU温度、NVME硬盘温度、SATA硬盘温度](https://h8cs-my.sharepoint.com/:u:/g/personal/od577_365a1_me/Ecs5ETyuagFBg_UakUPvtw0B9ubYaE8i7q55OffxvK5wMA?e=7tgPV2)             
* [ESXi-6.7.0-Update3B-2.5Gbps-customized](https://h8cs-my.sharepoint.com/:u:/g/personal/od577_365a1_me/EfQnLOjegrVOpm22T0Sm42MB7E3uObuLg9Y1LOJXi_3-yw?e=Avy8Cn)   
* [NAT路由类型检测工具NatTypeTester](https://github.com/HMBSbige/NatTypeTester/releases)     


## 教程区        

### passwall相关        

* [关于passwall的DNS问题](./tips/passwallDNS.md)          
* [不希望任何人的设备连到我的openwrt路由下都可以翻墙](./tips/NoFriendUSEmyFQ.md)
* [passwall指定特定设备走特定节点](./tips/passwallTeDingSheBeiQuanJuDaiLi.md)          
* [passwall指定特定网站走特定节点](./tips/passwallURLfenliu.md)         
* [BT下载不走代理、翻墙线路极限速率测试、守护进程](./tips/passwallAdvancedSetting.md)                   
* [帮助完善passwall的手动添加规则](./tips/helpPasswallProxyFile.md)     
* 可以使用负载均衡同样地实现故障切换功能
* 恢复默认配置方法，地址栏输入例：

```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/reset_config
```

* 隐藏菜单方法，地址栏输入例：
 
```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/hide
```

* 当你隐藏后想再次显示，地址栏输入例：

```
http://192.168.5.1/cgi-bin/luci/admin/services/passwall/show
```

* passwall芝麻开门命令（如果需要开门）：         
```
touch /etc/config/passwall_show        
```

### ssrp相关      

* [ssrp的分流如何开启](./tips/ssrpFenLiu.md)    
* [ssrp的翻墙线路莫名其妙变动](./tips/ssrpXJBbian.md)         
* ssrp芝麻开门命令（如果需要开门）：          
```
echo 0xDEADBEEF > /etc/config/google_fu_mode
```               

### 其他插件相关         

* [upnp相关问题整理](./tips/upnp.md)  
* [网关代理"旁路由"下访问国内网站缓慢甚至失败](./tips/PangLuYouGNM.md)                       
* [手动挂载移动硬盘/U盘](./tips/ManullyGuaZai.md)          
* [动态DNS中配置阿里云DDNS](./tips/ddns.md)
* [看一下是否需要打开外网访问路由后台](./tips/webadmin.md)
* [使用Samba协议打造家庭影音库](./tips/sambaNB.md) 
* [最强文件分享服务器FileBrowser](./tips/FileBrowserNB.md)
* [挂在路由上的百度网盘客户端](./tips/BaiDuWangPan.md)             
* [家里自建一个ssr服务端](./tips/ssrMDBServer.md)       
* [WAN口丢失后重建](./tips/CreWAN.md)

### 固件全新安装升级、不保留配置上传升级相关

* [不保留配置上传刷写固件](./tips/Upgrade.md) 
* [虚拟机+EFI固件安装问题汇总](./tips/VMandEFI.md)    
* [PE环境下写入固件到硬盘兼容性最好的v1.2版本DiskImg](./tips/PEwirteIMG.md)          
* [直写固件到U盘或硬盘或TF卡的最强唯一推荐软件：Rufus](https://github.com/pbatard/rufus/releases)        

## 其他区 

* [清理windows系统下DNS缓存](./tips/clearDNS.md)  
* [Chrome浏览器强制转换LuCI页面为暗黑主题](https://chrome.google.com/webstore/detail/dark-reader/eimadpbcbfnmbkopoojfekhnkhdbieeh?hl=zh-CN)      
* [路由下主机数据传输速率查看](./tips/HostSpeedMonitor.md)     
* [系统资源消耗实时监控查看](./tips/CPUandRAMmonitor.md)     
* [编译入门秘籍](./fishtool.md)    
* [几种加密算法下传输速度测试脚本](./sh/ss_test.md)      
* [单线程测速](http://speed.cloudflare.com)       
* [banner生成器](http://www.network-science.de/ascii)        
* [搬瓦工提供IP连通性测试](https://ping.pe)   
* [国内各省市对某网站ping检测](http://ping.chinaz.com)             
* [查询IP地址](http://www.ip111.cn)     
* [ip反查绑定过的域名](https://tools.ipip.net/ipdomain.php)      
* [GitHub各项服务状态](https://www.githubstatus.com)     
* [主流网站的可用状态](https://downdetector.com)        
* [telegram汉化简体(推荐第三方)](https://t.me/setlanguage/classic-zh)     
* [telegram汉化简体(官方测试版本)](https://t.me/setlanguage/zh-hans-raw)      
* [telegram汉化繁体(官方测试版本)](https://t.me/setlanguage/zh-hant-raw)        
* [禁止telegram垃圾广告群拉我入群](./tips/TGantiADpull.md)    
* [为什么我无法telegram私聊和在公开群发言？？？](./tips/TGchatForbiden.md)
* [下载telegram群文件的正确姿势](./tips/RuHeZhengQueXiaZaiTGFile.md)         
* [win10Home家庭版安装HyperV虚拟机](./tools/hyperVinstall.md)      
* [东东的屏保怎么弄的](./tips/DDMacHaiBao.md)    

## 常用命令、操作区

* 完全删除lede文件

```
rm -rf lede
```

* 清空回收站

```
sudo rm -rf ~/.local/share/Trash/*
```

* Windows的HOSTS文件位置(当出现一些网页元素加载失败时可以尝试清空HOSTS规则)

```
C:\Windows\System32\drivers\etc
```

* powershell中SSH连接路由器后台举例

```
ssh root@192.168.2.1
password
```

* openwrt恢复出厂设置命令

```
firstboot
```

* 修改LAN口IP

```
vi /etc/config/network
```

* 默认root进入系统后添加普通用户

```
sudo useradd -m zhangsan -s /bin/bash
sudo passwd zhangsan
sudo adduser zhangsan sudo
su zhangsan
cd /home/zhangsan
sudo apt-get update
sudo apt-get install vim
```

* 举例指定git拉取my-19.07分支

```
git clone -b my-19.07 https://github.com/Lienol/openwrt.git
```

* 显示隐藏文件（.config）

```
ls -a 
```

或 
Ctrl+H

* git冲突，放弃本地修改，直接覆盖

```
git reset --hard
git pull
```

* 强制安装上传到 /tmp/tmp 的IPK

```
opkg install /tmp/tmp/*.ipk --force-depends
```


## About区             
* [参考消息](https://t.me/openwrt_cn)
* [党支部](https://t.me/+bykW8ZpJax4wYzc1)                







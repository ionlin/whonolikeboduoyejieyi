![1](https://user-images.githubusercontent.com/73426989/121067643-e0606880-c7fd-11eb-8673-6a8747853c20.png)     

# 授人以鱼不如授人以渔        

这里是简短的编译OpenWrt入门秘籍。目前除了[ImmortalWrt](https://github.com/immortalwrt/immortalwrt) 缝合好了几大爬墙插件可供直接make编译，其他的Op分叉都或注释或分离或隐藏了。    

## 选择op分叉主体         

推荐：[coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)           

## 需要手动添加ssrp、passwall、openclash等插件      
        
此部分操作说明（保存编辑过的feeds.conf.default后此部分结束）：    
```
#在拉取的op分叉主体的源码的feeds.conf.default文件(lede目录下即可找到)中添加：  

src-git helloworld https://github.com/fw876/helloworld
#这是ssrp插件的最新库地址，只是库名字叫helloworld，包名字其实还是ssrplus这个比，安装好后是界面是shadowsocksR plus + 这个比，千变万化我是你爸...      

src-git passwall https://github.com/xiaorouji/openwrt-passwall   
#这是passwall插件的最新库地址，库名、包名、菜单名目前统一，之前菜单名是 科学上网、...还有什么名字瞎几把改的我忘了...      

src-git OpenClash https://github.com/vernesong/OpenClash
#这是openclash插件的最新库地址       

src-git lienol https://github.com/Lienol/openwrt-package
#这是Lienol的package库，里面有一些lede里没有的包      
```
              
## 接下来三步走

```
./scripts/feeds update -a
```
```
./scripts/feeds install -a
```
```
make menuconfig
```
        
## menuconfig怎么选        

如何选到你的设备，例如R2S、X86_64、ACRH17这些设备怎么选到，请你谷歌一下“xxx openwrt编译”，找几个博客看一下就知道位置在哪了...        
选好设备后，接下来几个你可能刚需的设置点：       

* Extra Packages > autocore、autosamba、automount、ipv6helper         
无论软硬路由都可勾选了，没坏处。         

* Network > Firewall > ip6tables > ip6tables-extra、ip6tables-mod-nat        
都勾了。         

* LuCI > Themes >          
一般不建议勾选bootstrap、material之外的主题。      

* LuCI > Applications >         
MTK MIPS架构的几个K2P、新三什么的必选mtwifi否则没无线信号,如果没看到mtwifi选项那就无所谓了，可能大雕调整了mtwifi的位置并且默认选上了，你不用操心了。          
其他的软路由无需操心wifi驱动。                   
硬路由一般爬墙插件类只勾选ssrplus : ssr client + xray (xray兼容v2ray、trojan、ss，硬路由勾选ssrp下面这两个就够用了，再多K2P一定超空间出不来固件)       
其他的爬墙插件则不建议为硬路由勾选。 
还有一些adbyby plus什么的几把玩意就别为硬路由勾选了,软路由也没必要勾选，去广告本来就不可避免有误伤。            
软路由就无脑ssrp全勾+passwall全勾+openclash全勾+其他你知道的用过的一些什么各种文件服务器、VPN服务端、qos、TTYD、uu加速器......眼熟的都可以选，不熟的别选。               

![1](https://user-images.githubusercontent.com/73426989/121642667-69f48c80-cac3-11eb-9034-e67292c4a701.png)        

[返回主页](https://boduoyejieyi666.github.io/whonolikeboduoyejieyi/)        

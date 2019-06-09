![DJY](Images/LOGO.jpg)


****
其他语言(翻译来自@Noob-DaoXin 道心 等待翻译中.....): [English](README_EN.md)

* [点击我查看HTML版本介绍](https://johanlike.github.io/DJY-Oneplus6-or-Oneplus6T-Nethunter-Andrax-Kernel/)

# 目录
* [介绍](#介绍)
* [目前已知BUG](#目前已知BUG)
* [Magisk拓展增量包](#magisk拓展增量包)
* [安装教程](#安装教程)
* [常见问题解决](#常见问题解决)
* [相关代码和致谢列表](#相关代码和致谢列表)
* [联系方式](#联系方式)


****
# 介绍
大家好我是来自中国的业余玩家ID：***DJY***喜欢唱，跳，Rap，打篮球！!(就是一个打酱油的菜鸟的意思....)

<div align=center>![CXK](Images/CXK.gif)

这是一个支持Kali ***Nethunter***和***Andrax***的全功能内核。适用于***oneplus6***和***oneplus6T***。基本和一台可移动小型Linux差不多，包含了大多数的主流的功能和特性：

* 当前版本DJY-Kernel-V66
* aarch64-gcc-10编译（2019-6.03）
* 采用Elementalx内核配置文件为基础来构建内核以确保速度和稳定性（2019-6-5 ElementalX-OP6-3.17 ）
* 合并上游Linux代码以确保代码为最新（目前版本V4.9.180）
* 并将Linux官网的主流无线固件编译进内核当中以确保airmon-ng正常注入（rt2561.bin  mt7601u.bin  rt3290.bin  rt3071.bin  rt73.bin  rtlwifi/rtl8192eefw.bin  rtlwifi/rtl8821aefw_wowlan.bin  rtlwifi/rtl8188eufw.bin rtlwifi/rtl8188efw.bin rtlwifi/rtl8192cfwU.bin  rtlwifi/rtl8192cfwU_B.bin  rtlwifi/rtl8192cufw_TMSC.bin  rtlwifi/rtl8192cufw_A.bin  rtlwifi/rtl8192cufw.bin  rtlwifi/rtl8821aefw.bin  rtlwifi/rtl8192sefw.bin  rtlwifi/rtl8192cfw.bin  rtlwifi/rtl8192eu_nic.bin  rtlwifi/rtl8192defw.bin  rtlwifi/rtl8192cufw_B.bin  rt2561s.bin  rt2661.bin  rt3070.bin  rt2870.bin  rt2860.bin  carl9170-1.fw  ath9k_htc/htc_9271-1.4.0.fw  ath9k_htc/htc_7010-1.4.0.fw  ar7010.fw  ar7010_1_1.fw  htc_9271.fw）

****

* Elementalx 内核特性支持
* Selinux 永久设为Permissive状态
* HID攻击支持
* Droidducky攻击支持
* Rndis手机OTG嗅探电脑数据支持
* Hackrf 支持
* Rtl-SDR 支持
* BladefRF 支持
* Yard stick one 支持
* Ubertooth 支持
* LimeSDR支持
* USRP 支持
* Hackrf USRP RTL-SDR BladeRF LimeSDR UHD驱动支持
* OTG蓝牙攻击支持
* Mousejack支持
* 外接各种红外设备支持
* PN532 支持
* Chameleon-Mini 变色龙支持
* Proxmark3 HID驱动支持
* Proxmark3 CDC驱动支持
* 外接pppoe线缆嗅探各种类型路由器
* Lan-tap支持
* 支持各种外接线缆
* PLC设备转接支持
* Osmocombb OTG C118 C119（RF设备）支持
* OpenBTS C118 （RF设备）支持
* 解锁NFC全功能支持（需要应用APP二次开发）
* 解锁内置AM/FM信号支持（需要应用APP二次开发）
* 键盘和鼠标支持插上即可用
* TTL转接USB 蓝牙，树莓派，ESP8266(WIFI HID攻击支持)等设备支持
* 各种转接线例如：PL2303，CP210X，CH340..等转接线支持
* 各种转接头支持： SMA，HDMI，TNC..等接头支持（部分接头需要手工焊接转换）
* 内核刷机包自动安装Magisk功能（暂时不完美待修复）
* 自定义开机动画支持

****

* 其他功能和设备支持待发掘反馈.........

****

* [点击我查看部分功能测试截图和视频](https://johanlike.github.io/DJY-Oneplus6-or-Oneplus6T-Nethunter-Andrax-Kernel/Images/)

****

***欢迎其他功能和设备支持反馈，以便记录内核的功能性。你的支持是我最好的动力，欢迎Star***

# 目前已知BUG

# 相关代码和致谢列表

***特别致谢@simonpunk对HID修补的大力支持。用到的相关构建代码链接***：

https://github.com/simonpunk/nethunter-app

https://github.com/pelya/android-keyboard-gadget

https://github.com/simonpunk/Android-Terminal-Emulator

***感谢@draguve HID攻击相关开源优秀项目***

https://github.com/draguve/droidducky-app

***感谢@kristofpetho优秀开源的内核代码***

https://github.com/kristofpetho/op6

***这是我已经修复的内核源码，已修复HID和WIFI并将Selinux 永久设为Permissive状态，长期合并Linux官网代码保持最新和将常用无线固件注入到内核中***

https://github.com/johanlike/DJY-Nethunter-Andrax-Kernel-Source

***感谢@meefik @chrisk44 @draguve @simonpunk对以下代码做出的贡献，以下相关Apps代码使用Android Studio 3.6Canany3(191.5618338)编译于2019-6-9***

https://github.com/meefik/linuxdeploy.git

https://github.com/chrisk44/Hijacker.git

https://github.com/draguve/droidducky-app

https://github.com/simonpunk/nethunter-app

https://github.com/simonpunk/Android-Terminal-Emulator






# 联系方式
***Kali Linux QQ交流群：712420808(欢迎各种大佬进群吹水)***

***电报群组：https://t.me/nethunter666 (欢迎各种大佬萌新进群吹水)***

***请尊重作者劳动成果,这样才能共同进步(希望国人团结...)如果你需要转载请注明出处谢谢.***

# GA-H170MSTX-DATTO-O3
云轩H170 OpenCore0.6.0 引导文件（2020年9月6日更新上传）
  
1.硬件配置：  
cpu：i7 8700 es(qn8g)  
内存：协德 2666 8g*2  
硬盘：M.2 2280 十铨 512G  
wifi蓝牙：DW1820A  
声卡：ALC255   
显示器：自行组装15.6寸 4K便携显示器 minihdmi接口  
键鼠：罗技K580+M590  
  
2.硬件使用情况：所有硬件均正常工作
我的无线网卡1820A设备信息是pci14e4,43a3，请用Hackintool查看你自己的型号做相应修改    
详细教程参见@黑果小兵的教程[DW1820A/BCM94350ZAE/BCM94356ZEPA50DX插入的正确姿势](https://blog.daliansky.net/DW1820A_BCM94350ZAE-driver-inserts-the-correct-posture.html) 

3.已知问题：用本引导文件尝试在外置硬盘安装Big Sur失败后，进入Catalina wifi驱动丢失，解决方式关机断电重新开机后恢复正常  
无线网卡建议使用白果网卡  
白果网卡用户可删除AirportBrcmFixup.kext、BrcmBluetoothInjector.kext、BrcmFirmwareData.kext、BrcmPatchRAM3.kext这四个驱动并对应修改config.plist
  
4.CFG Lock：使用此引导必须解锁CFG Lock，本人使用grub进行bios修改，拔了主板电池后该功能会失效，需重新解锁CFG Lock
  
5.BIOS版本：本人使用的是[SMX Diy论坛](http://www.smxdiy.com/) @dsanke 基于官方F21版本修改的bios，在此感谢@dsanke大佬

6.[BIOS设置请参考我的张大妈](https://post.smzdm.com/p/ag827k43/)
  
7.致谢：在此特别要感谢@[黑果小兵](https://blog.daliansky.net/) 、@[Xjn](https://blog.daliansky.net/OpenCore-BootLoader.html)写的教程，没有他们的教程，oc引导是无法完成的  

8.系统版本：目前使用 Catalina 10.15.6

9.注意：引导文件里删除了机型配置，请用OCC配置工具修改config.plist，可以使用imac和Macmini对应的机型，请自行测试。本人使用imac19,2

10.写在最后：上一次做的oc引导是2020年1月份的事儿了，我的云轩闲置了半年，一直没机会用，10.15.4之后的版本HDMI一定要仿冒显卡之后才能进系统，所以我的主机停留在10.15.3版本很久
最近Lilu.kext和WhateverGreen.kext都更新了，顺带更新了opencore版本，换了EFI后先用外置硬盘新装了10.15.6测试可以进系统后，用原硬盘直接升级至最新系统，目前HDMI正常工作

欢迎云轩H170用户使用测试转载，感谢你们的支持！

2020年9月16日，我的云轩已经售出，0.6.0就是我最后更新的版本了。

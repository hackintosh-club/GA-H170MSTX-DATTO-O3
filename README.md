# GA-H170MSTX-DATTO-O3
云轩H170 OpenCore0.6.0 引导文件  
  
1.硬件配置：  
cpu：i7 8700(qn8g)  
内存：协德 2666 8g*2  
硬盘：M.2 2280 十铨 512G  
wifi蓝牙：DW1820A  
声卡：ALC255  
  
2.硬件使用情况：所有硬件均正常工作
我的1820A是pci14e4,43a3，请用Hackintool查看你自己的型号做相应修改
已知问题：如遇到wifi或丢失蓝牙，关机断电重启后恢复正常（此情况应该比较少见），建议使用白果网卡
白果网卡用户可删除AirportBrcmFixup.kext、BrcmBluetoothInjector.kext、BrcmFirmwareData.kext、BrcmPatchRAM3.kext这四个驱动
  
3.特别说明：使用此引导必须解锁CFG Lock，本人使用grub进行bios修改，拔了主板电池后该功能会失效，需重新解锁CFG Lock  
  
4.BIOS说明：本人使用的是SMX Diy论坛 @dsanke 基于官方F21版本修改的bios，在此感谢@dsanke大佬  
  
5.致谢：在此特别要感谢@黑果小兵、@Xjn写的教程，没有他们的帮助，oc引导是无法完成的  

6.系统：Catalina 10.15.6

7.写在最后：上一次做的oc引导是2020年1月份的事儿了，我的云轩闲置了半年，一直没机会用，10.15.4之后的版本HDMI一定要仿冒显卡之后才能进系统，所以我的主机停留在10.15.3版本很久
最近Lilu.kext和WhateverGreen.kext都更新了，顺带更新了opencore版本，换了EFI后先用外置硬盘新装了10.15.6测试可以进系统后，用原硬盘直接升级至最新系统，目前HDMI正常工作

# Clover-EFI-For-Dell-5577

  从2018年10月1日利用课下时间折腾Hackintosh，断断续续，中间也曾因配置文件不完美放弃折腾投奔*ArchLinux*，最后还是遵循了真香定律（手动滑稽）。  
  双十二弃Linux，回归黑果，以前没能解决的问题不知道为什么突然解决了，也就顺其自然地折腾好了属于自己电脑的Clover文件，分享一下。  
  ### 这份EFI配置文件不全是自己的劳动成果，其中结合了很多前辈的Clover配置文件  
  * 黑锅小兵大大 **macOS Mojave 10.14.2 18C54 正式版 with Clover 4792原版镜像** 中含有的EFI配置文件 
  * Dell 7520（好像是这个，具体型号忘记了...）  
       可能是DELL主板有相似之处吧，这个型号完美EFI的其中一部分文件在我的本子上是可用的  
  * Dell 5577在*osx 10.13*下的EFI文件。   
  
  *（感谢前辈们的劳动成果了，谢谢鸭~）*
  
    进入GitHub，从这里用到了不少东西，也学到了很多，此次也算是对这个环境的一份贡献吧。

## 本人配置

 硬件类型|型号
 ---- | ----- 
 笔记本型号|Dell 5577 (Inspiron 15pr-5645b)
 CPU|Intel Core i5-7300HQ
 内存|镁光 英睿达 8G 2400Mhz x 2
 SSD|SAMSUNG SM951 512G M.2 NVME
 HDD|西数 1T
 显卡（***已屏蔽***）|NVIDIA GTX1050 4G
 板载网卡|Realtek RTL8168H/8111H PCI Express Gigabit Ethernet
 无线网卡|DW1560/BCM94352z 802.11ac Wireless Network Adapter
 声卡|Realtek ALC 256
 显示屏|京东方 15.6 IPS 72色域
 
  本人也是先后折腾了不少硬件（也有折腾黑苹果之前换的），所以总体配置也是和笔记本原版配置有所差别，不过感觉除了网卡（***BCM94352z***），换的硬件都是对无关紧要的，同型号食用应该问题不大。

## 瑕疵
* 开机到苹果标志进度条在头部偶尔闪退，再开一次机才可完美读条
* 键盘出现过一次睡眠后唤醒后不能用的情况（USB外接键盘可用，猜测是PS2的问题），重启就好了，但是再也没出现过就没再管
* 系统自带菜单栏电池百分比不会自动更新，用第三方软件却可以更新；偶尔开机需手动打开菜单栏
* 刚开机耳机插孔不能用，需睡眠唤醒才可用
* 键盘FN仍不能调节亮度（在系统快捷键中手动设置快捷键可调节）

      自我认为不存在完美的黑苹果，无法判断我的Clover配置文件完美程度，所以没用***xx%完美黑苹果***来写简介。

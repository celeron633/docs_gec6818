# GEC6818（S5P6818）启动文件（包含bl部分和uboot）


bl1-mmcboot-sd.bin：按ARM ATF规范，这个是bl2，被芯片内部的bootrom（bl1）启动，这个适合写入sd卡的场景。

bl1-mmcboot-emmc.bin：和上面一样，只是适合用于写入GEC6818自带的EMMC的情况下使用。

fip-loader.img：bl31，这个是没有源码的。

fip-secure.img：bl32，这个也没有源码。

fip-nonsecure-GEC6818.img：bl33，也就是uboot，这个适合粤嵌的GEC6818开发板

fip-nonsecure-FriendlyARM.img：和上面一样，适合nanopi3，nanopc-t3，nanopc-t3-plus

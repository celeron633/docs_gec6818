# GEC6818 boot分区备份

这个boot.tar.gz里面的数据需要写到boot分区里面去，比如boot分区sdb1挂载在了mnt，使用下列命令还原回去（boot.tar.gz就不要放在mnt下面了，直接放自己HOME目录下即可）：

```shell
sudo tar -zxvp --xattrs -f boot.tar.gz -C /mnt
```

写入完成以后，umount，然后sync，再拔掉sd卡：

```shell
sudo umount /mnt
sync
```

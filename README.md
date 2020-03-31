# HowToBuildPlexServer

## 1、格式化移动硬盘

`umount /dev/sdc`

`mkfs.ext4 /dev/sdc1(x替换为你的adbc等，你可以用fdisk -l 命令查看)`

## 2、把移动硬盘挂载到/mnt下

`mount -t ext4 /dev/sdc1 /mnt`

## 3、把docker复制 /mnt 下
`cp -a /opt/docker /mnt`

## 4、把移动硬盘卸载

`umount /dev/sdc1`

## 5、回到web 界面,要在luci界面操作

 `mount 分区到/opt/ （划重点！）`
 
## 6、重启路由器 （划重点！）

---
layout: post
title: "57期 - Create an Encrypted USB Stick"
date: 2012-09-22 13:35
comments: true
categories: HOW-TO
---

Written by Kalven Slade
作者：Kalven Slade

Many articles seem to focus on using various utilities such as UNetbootin or Universal USB Installer from pendrivelinux.com, but none of these are necessary to install Ubuntu on a USB hard disk or flash drive, and they don't account for the possibility of losing your portable OS, which may contain personal information.

在pendrivelinux.com的网站上，很多文章都是专注于如何用UNetbootin或者Universal USB Installer 等类似工具创建安装有Ubuntu的移动硬盘或者USB闪存。但是他们并没有考虑到：如果你把存有个人隐私的移动硬盘或闪存丢失了，你的隐私将有可能受到侵犯。

This guide will walk you through how to create an encrypted portable OS that will allow you to have a secure device where you can update and store files.

本教程将跟你一起创建一个加密的移动OS，让你存得安心，用得放心。即使丢了，就随它去吧。因为它是经过加密的，别人无法获得你的私人数据。

Everything in the document assumes that you are doing a fresh install of Ubuntu 10.04.2 (11.10 has also been tested to work,) and doing each step in order. This guide will also be easier to follow if you disconnect any other drives including internal ones except the CD/DVD. (If your other drive remains, make sure you place Grub on the correct disk!)

本教程假设你以全新的方式安装Ubuntu 10.04.2（经测试，兼容11.10），如果你可以将其他内置驱动器拔出，仅留下CD/DVD设备，你会更容易操作。（如果你有其他驱动器，请确保GRUB中指向的是正确的磁盘）

With this being a portable OS, using Xubuntu will make it faster on flash drives, and allows it to function on computers with lower memory requirements than Ubuntu.

从便携式OS的角度来说，Xubuntu会比Ubuntu运行得更快，因为它需要更少的内存。

Encryption will help you secure your data if you lose or have your computer stolen.

如果你的电脑被偷，加密可以保证你的数据安全。

Ubuntu has built in support for two types of encryption by default, using the Alternate Install CD: full disk encryption, and profile/home encryption. You can add additional encryption using TrueCrypt.

Ubuntu默认内置两种加密方式，使用CD的自定义方式安装：整个硬盘进行加密，或者仅仅是个人文件和家目录进行加密。你可以使用TrueCrypt进行额外的加密设置。

A USB flash can be slow (sometimes too slow!); a USB or ESATA hard drive will function much better.

使用USB闪存会很慢（有时候会非常慢！）；USB或者ESATA硬盘会好一些。

Linux, unlike Windows, can easily be moved from computer to computer, and boot from your portable drive.

Linux不像Windows，Linux可以很简单的从一个电脑换到另一个电脑，直接由移动设备启动即可。

Try to stay away from restricted features like 3d video support on your portable install.

在安装移动OS的时候，请尽量不要设置限制性的特性，例如3d图像支持。

Boot the Alternate Install CD for Ubuntu or Xubuntu, and choose install from the menu.

选择Ubuntu或者Xubuntu系统，从CD启动，在选项中选择自定义方式安装。

Unless you need to modify settings, just choose the defaults for your language, location, keyboard configuration, host name, and time zone.

除非你需要修改一些设置，在语言、地区、键盘设置、域名、时间等部分直接选择默认即可。

Setting up your partitions is very important, and probably the hardest part to do correctly. You want to limit how often the drive is both read and written to; encryption adds a bit of overhead. EXT3 and EXT4 are too slow, also having a swap space will cause speed issues as well. I have found that it is best to create a FAT32 Partition for sharing files between Windows computers, and using EXT2 for your Ubuntu install.

设置硬盘分区参数非常重要，同时也是最难的一部分。你需要计算出你电脑对读写的需求；硬盘的加密会增加硬盘的工作负荷。EXT3和EXT4太慢啦，而且swap分区会更加影响速度。所以我们选择使用EXT2作为我们的主分区用来装Ubuntu，然后使用FAT32的分区用来和Windows共享文件。

Choose manual from the partition menu. Choose your USB drive (and not any existing partitions), and press Enter. It will ask you if you want to create an empty partition table on this device. Choose yes.

在分区菜单中选择手动。选择你的USB磁盘（不要选择现有的分区），点击确认。之后它会询问你是否在这个设备上创建一个空分区表，选择是。

Below your drive, it should now be listed as free space. Choose it and create a new partition. This new partition will be your FAT32 partition for Windows transfers. I have a 16 GB flash drive, and choose to allocate 3 GB for my FAT32 partition. Make it a Primary partition, at the beginning of the disk. Change the file type to FAT32, and mount point to none. Then choose done setting up this partition.

在列表中，你应该能够看到空闲的空间。选择此空间然后新建分区。分区格式为FAT32，用于和Windows之间传输数据。我的闪存是16G，我将3G分配成为FAT32的分区。将其设置为从头开始的主分区，挂载点选择无，然后确认。

Now we can create the Boot partition, choose your free space again, and create a new partition, 256 MB is good. Make sure you change from GB (Gigabytes) to MB (Megabytes), or you may not have enough space for your OS. Make it a Primary Partition at the beginning of the disk. Change the File system to EXT2, mount point to /boot, and bootable flags to on. Now you can choose done setting up this partition.

现在我们开始新建启动分区，选择空闲空间，新建一个256M的主分区。确定单位是MB而不是GB，否则你将不够空间。分区格式为EXT2，将其标记为活动分区，挂在在/boot下。点击确认即可开始下一步。

From the remaining free space, create a new primary partition with Physical volume for encryption as the file type, then choose done setting up this partition.

选择剩下的全部空闲空间，创建一个主分区、设置为物理卷，并点选加密。确认。
Choose Configure encrypted volumes from the menu, yes to write changes to the disk. Choose Create encrypted volumes, choose finish.

在菜单中选择配置加密卷，选择是，确认创建加密卷。

Create a password and verify.

创建密码，并确认。

You will now be back to the partitioner, and you will see a new encrypted volume drive is listed, select the partition (it will will have a file system of EXT4), and press enter.

现在你会回到分区界面，你可以看到你的加密分区呈现在列表当中，选择此分区（默认是EXT4格式的分区），按下回车。

Change the file system to EXT2, mount point to `/`, and choose done setting up partition.

将文件系统格式改为EXT2，挂在在/下。确认。

Choose finish partitioning and write changes to disk.

选择完成，并将更改写会磁盘。

Choose no when you see the warning about a missing mount point for the FAT32 partition and the missing SWAP partition, then yes to write changes to the disk.

提示没有为FAT32的分区设置挂载点，以及没有SWAP分区，选择否。然后选择确认。

Continue with the install, do not choose home directory encryption for flash drive installs.

继续安装，不要选择家目录加密。

Once installed, run updates, and reboot, then you’re done!

安装完成之后，更新，重启。完成。

## Encryption Info

##加密信息

You can change and add passwords for your full disk encryption - 8 passwords are allowed, and they are numbered 0-7.

你可以为你整个磁盘更变或增加加密密码 - 你可以设置8个密码，分别为0 - 7号密码。

To see which keys are in use:

    sudo cryptsetup luksDump /dev/<drive>

你可以查看那些字串已被使用：

    sudo cryptsetup luksDump /dev/<分区>

Changing Your Password

更变密码

To change your password you will need to first add a new one, and then remove the old one.

你需要先增加一个新密码，然后才能删掉旧的密码。

Step 1: Add New Password:

    sudo cryptsetup luksA    ddKey /dev/<drive>

步骤1：新增一个密码：

    sudo cryptsetup luksA    ddKey /dev/<分区>

Enter any passphrase: <your current password>

输入任意密码：<你现在的密码>

Enter new passphrase for key slot: 

输入新密码：

Verify passphrase: 

验证：

Step 2: Remove Old Password:

步骤2：移除旧密码：

run a dump again to verify key slot added:

    sudo cryptsetup luksDump /dev/<drive>

    sudo cryptsetup luksKillSlot /dev/<drive> <key slot number>
    
首先验证新密码已经成功创建：

	sudo cryptsetup luksDump /dev/<分区>
	sudo cryptsetup luksKillSlot /dev/<分区> <密码序列>

Enter any remaining LUKS passphrase: 

输入其他的LUKS密码：

Verify removal with another dump:

    sudo cryptsetup luksDump /dev/<drive>
    
确认删除成功：

	sudo cryptsetup luksDump /dev/<分区>

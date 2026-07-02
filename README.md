# PyTextOS

**Welcome to the PyTextOS™ 1.0 operating system!**

PyTextOS is a text-based operating system that can run on 64-bit and legacy 32-bit systems. It has a text editor, a calculator, an account manager, a simple game, and much more. It uses multi kernel technology.

---

## Table of contents
- [Compatibility](#compatibility)
- [Download](#download)
- [Setup](#setup)
- [Installation](#installation)

---

## Compatibility
PyTextOS is compatible with a wide range of computers. It can even run smoothly on a computer from the XP era.

It can:
- Run smoothly on old and new computers
- Run on 64 and 32 bit systems
- Run from a Live CD or USB

## Download
To download the operating system, go to to [the latest release](https://github.com/SpockTech/PyTextOS/releases/tag/release) and download the `.iso` file. Now that you have the file, you can un it on a vitual machine or on real hardware.

## Setup
Follow the steps to run the operating system in a virtual machine.
1. Download [QEMU](https://www.qemu.org/download/)
2. Install QEMU
3. Run `qemu-img create -f qcow2 my_disk.qcow2 20G` in your Linux terminal. On windows, press WIN+X and select `Terminak (Admin)`. Make sure your ISO is in the same location as the `.qcow2` file.
4. Run `qemu-system-x86_64 -hda my_disk.qcow2 -cdrom PyTextOS.iso -boot d -m 4096M -enable-kvm` and install PyTextOS following the [Installation](#installation) section.

Follow the steps to run the operating system on real hardware
1. Get a USB (8 GB or bigger)
2. Download the latest version of [rufus](https://rufus.ie/en/)
3. Select the ISO in rufus and create the bootable USB.

---

## Installation
Installing PyTextOS is pretty easy. You just need to follow the steps to install the operating system. You need to boot into your PyTextOS USB before you can start installing the operating system.

You wil see the PyTextOS prompt `PyLiveCD> `. It is the full PyTextOS operating system running in your computer RAM. It is not installed yet, which means you need to type `setup` and hit ENTER to enter the setup.

After typing `setup`, you must follow the steps to install PyTextOS to the storage device.
1. The screen will go blank, then it will say `Stating PyTextOS Setup...`. This will take a few seconds.
2. You will be prompted to select which drive you want to put PyTextOS in. Example below:
   ```
   Selet where to install PyTextOS:
     Disk/partition              ##  Size
     ------------------------------------
     SATA SSD (partition 0)      1   20 GB
     SATA SSD (partition 1)      2   31 GB
     IDE Hard Drive              2   500 GB
   ```
3. You will be prompted to create up to 5 user accounts with passwords. Just press ENTER to proceed.
4. Once you have created the user profiles, PyTextOS will copy the files to your drive and create all the directories.
   It will display something like:
   ```
   Successfully copied file: /system/boot/boot.asm
   Successfully copied file: /system/kernel/vmlinuz64bit
   Successfully copied file: /system/kernel/vmlinuz32bit
   ```
6. You are prompted to create a password to access the account manager.
7. After creating a password, you can now start using PyTextOS.

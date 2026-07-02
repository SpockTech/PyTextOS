# PyTextOS

PyTextOS is a text-based operating system that can run on 64-bit and legacy 32-bit systems. It has a text editor, a calculator, an account manager, a simple game, etc. The OS binaries will not be released as this OS will be kept closed source. It will go open source soon after a few versions.

---

## Compatiblility
PyTextOS is compatible with a wide range of computers. It can even run smoothly on a computer from the XP era.

It can:
- Run smoothly on old and new computers
- Run on 64 and 32 bit systems
- Run from a Live CD or USB

## Download
To download the operating system, go to to [the latest release](https://github.com/SpockTech/PyTextOS/releases/tag/release) and download the `.iso` file. Now that you have the file, you can un it on a vitual machine or on real hardware.

Follow the steps to run the operating system in a virtual machine.
1. Download [QEMU](https://www.qemu.org/download/)
2. Install QEMU
3. Run `qemu-img create -f qcow2 my_disk.qcow2 20G` in your Linux terminal. On windows, press WIN+X and select `Terminak (Admin)`. Make sure your ISO is in the same location as the `.qcow2` file.
4. Run `qemu-system-x86_64 -hda my_disk.qcow2 -cdrom PyTextOS.iso -boot d -m 4096M -enable-kvm` and install PyTextOS following the [Installation](#installation) section.

Follow the steps to run the operating system on real hardware
1. Get a USB (8 GB or bigger)
2. Download the latest version of [rufus](https://rufus.ie/en/)

---

## Installation

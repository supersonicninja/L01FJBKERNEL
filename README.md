L01FJBKERNEL
============
Introduction
 This is a kernel for the LG G2 Japanese variant "L01F11k"
 This kernel is for the stock JB ROM. Will not work on any AOSP ROMs.
 The objectives are to keep all stock features while adding new features and to improve performance, battery life and to reduce bugs.

Features
 -CCsecurity disabled to allow permanent root.
 -O3 compiler optimized.
 -Ondemand CPU governor tweaked and enabled by default.
 -Intellidemand CPU governor.
 -Simple GPU governor enabled by default.
 -Voltage adjustable.
 -SIO I/O scheduler enabled by default.
 -Various improvements and fixes.

Changelog
 See github commit log.

Building
 Install Ubuntu linux 64bit. Can be a virtual machine.Be sure to have 10GB+ HDD space left.
 Install the needed libs by typing the following command in the terminal emulator "sudo apt-get install git make". Type your user password when prompted.
 Download the android-ndk and find the google gcc 4.6. Then set it up by typing the following command in the terminal emulator "export CROSS_COMPILE=yourpathtothendk/bin/arm-eabi-".
 Download the kernel source by typing the following command in the terminal emulator "git clone https://github.com/supersonicninja/L01FJBKERNEL"
 Type the following command in the terminal emulator to navigate to the kernel directory "cd L01FJBKERNEL".
 Type the following command in the terminal emulator to configure the kernel as you wish "make xconfig".
 Type the following command in the terminal emulator to build the kernel "make"

Issues
 Will not build with gcc4.7+ or the linaro toolchain.
 dt.img compilation broken.

Credit
 LGE, Google and Linux devs for making the original kernel.
 glewarne for making the stockmod kernel for the LG G2. My kernel is sort of a port of the work.
 faux123 for the performance improvements.
 And many others!

Contact
 supersonicninja@xda

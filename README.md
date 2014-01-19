CyanogenMod 7 device configuration for the Huawei c8650

Powered by ferhung

HOW-TO BUILD:
============

Based on Ubuntu 10.10

1)Download and install repo:

$ mkdir ~/bin

$ PATH=~/bin:$PATH

$ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

$ chmod a+x ~/bin/repo

2)Download the source:

$ mkdir ~/android/system/

$ cd ~/android/system/

$ repo init -u git://github.com/CyanogenMod/android.git -b gingerbread

$ repo sync -j16

3)Download the rommanager:

$ ~/android/vendor/cyanogen/get-rommanager

4)Copy the device configuration to ~/android/system/device/huawei/c8650. Then build:

$ cd ~/android/system

$ . build/envsetup.sh && brunch c8650

5)Installing:

If the build was successful, you can now take the update zip found in out/target/product/c8650/ and flash using a custom recovery. Make sure to grab the latest Gapps to complete the experience.

# android_chroot_linux
Chroot linux from android

### Installation
 - Get root on android.
 - Install busybox ( [https://github.com/zacthespack/LinuxonAndroid-App/](https://github.com/zacthespack/LinuxonAndroid-App/)  (recommended) )
 - Get linux image for desired architecture.
 - Install script on sdcard
```sh
adb shell mkdir /sdcard/.bin
adb push ./bootscript.sh /sdcard/.bin/bootscript.sh
```

### Usage
From command line:
```sh
su -c sh /sdcard/.bin/bootscript.sh -i /sdcard/ubuntu/ubuntu-13.10.SMALL.ext2.img
```

From adb:
```sh
adb shell su -c sh /sdcard/.bin/bootscript.sh -i /sdcard/ubuntu/ubuntu-13.10.SMALL.ext2.img
```

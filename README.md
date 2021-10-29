acdbextract
========

This binary load the stock audio hal and dump the acdb table

#### Make sure you are on Stock Rom with Unlocked Bootloader  
#### Type following in adb terminal or cmd :
0. `adb reboot recovery`
0. `adb push acdbextract /system/bin`
0. `adb shell`
0. `cp /vendor/lib/hw/audio.primary.sdm660.so /system/lib`
0. `cp /vendor/lib/libaudio_log_utils.so /system/lib`
0. `cp /vendor/lib/libtinycompress.so /system/lib` or  
0. `cp /system/lib/vndk-29/libaudioroute.so /system/lib`  
    or `cp /system/apex/com.android.vndk.current/lib/libaudioroute.so /system/lib`
#### Install Magisk and termux.
0. Install Any root explorer file manager and give root permission.
0. Open termux with root permission.
#### Now Type below commands in termux.
0. `su`
0. `cd /`
0. `acdbextract > /sdcard/acdbids.txt`
0. Check `acdbids.txt` inside internal storage for required table

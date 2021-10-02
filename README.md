acdb_get
========

This binary dload the stock audio hal and dump the acdb table

0. Make sure you are on Stock Rom with Unlocked Bootloader
0. `adb reboot recovery`
0. `adb push acdbextract /system/bin`
0. `adb shell`
0. `cp /vendor/lib/hw/audio.primary.sdm660.so /system/lib`
0. `cp /vendor/lib/libaudio_log_utils.so /system/lib`
0. `cp /vendor/lib/libtinycompress.so /system/lib`
0. `cp /system/lib/vndk-29/libaudioroute.so /system/lib`
0. `./system/bin/acdb_get > /sdcard/acdbids.txt`
0. Check `acdbids.txt` for required table

acdb_get
========

This binary dload the stock audio hal and dump the acdb table

0. Make sure you are on MIUI
0. `adb reboot recovery`
0. `adb push acdb_get /system/bin`
0. `adb shell`
0. `cp /vendor/lib/hw/audio.primary.sm6150.so /system/lib`
0. `cp /vendor/lib/libaudio_log_utils.so /system/lib`
0. `cp /vendor/lib/libaudioroute_ext.so /system/lib`
0. `cp /vendor/lib/libtinycompress.so /system/lib`
0. `cp /system/lib/vndk-29/libaudioroute.so /system/lib`
0. `./system/bin/acdb_get > /sdcard/acdbids.txt`
0. Send `acdbids.txt` to me on Telegram or whatever

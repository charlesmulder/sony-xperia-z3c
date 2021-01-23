# Sony Xperia Z3 Compact

Build nr: `23.0.1.A.5.77`
Model nr: `D5803`

Just use [Sony EMMA](https://software.sonymobile.com/www/)

## Upgrade to build 23.5.A.1.291

- [Unlock Phone](https://developer.sony.com/develop/open-devices/get-started/unlock-bootloader/)
- [Sony Xperia Flash Tool](https://developer.sony.com/develop/open-devices/get-started/flash-tool/)

## General

```
# Dial *#*#7378423#*#* to access the service menu.
# Tap Service info > Configuration
# IMEI: 357652065063932
# Unlock code: EEE83C2C2DC2499D
# ensure device is listed
adb devices -l
# reboot
adb reboot bootloader
# ensure device is listed
fastboot devices
# unlock bootloader
fastboot oem unlock 0x<insert your unlock code>
```

```sh
# ensure device is listed
adb devices -l
# reboot
adb reboot bootloader
# ensure device is listed
fastboot devices
# unlock bootloader
fastboot oem unlock 0x<insert your unlock code>
fastboot flash recovery twrp-3.0.2-1-z3c.img
fastboot reboot
```

## Resources

- [Sony Open Devices](https://developer.sony.com/develop/open-devices)
- [Install LineageOS on z3c](https://wiki.lineageos.org/devices/z3c/install)
- [Flashtool](http://www.flashtool.net)
- [Xperifirm](https://xperifirm.com/)
- [TWRP for Sony Xperia Z3 Compact](https://twrp.me/sony/sonyxperiaz3compact.html)

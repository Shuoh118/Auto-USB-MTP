# Auto USB MTP

Xposed/LSPosed module: automatically switches the USB connection mode to MTP once the cable is plugged in, so you never have to pull down the notification shade and pick it by hand again.
-----
[中文](README.md)

## Features

- Automatically switches the USB mode to MTP after the data cable is plugged in
- Hooks UsbDeviceManager and AdbService, taking effect at the system_server layer

## Requirements

- Android 12 or above (module minApiVersion / targetApiVersion = 102)
- LSPosed (Zygisk or Riru)
- Root access (KernelSU or Magisk)

## Installation

1. Download the latest APK from Releases
2. Open the LSPosed manager after installing
3. Enable Auto USB MTP in the module list
4. Tick the System Framework (system) scope
5. Reboot the device

## Configuration
Changes are written immediately and take effect the next time the cable is plugged in.

## Changelog

### v2.0
- Fixed an issue where the cable could not be detected when it was repeatedly plugged and unplugged within a short time
- Reduced the APK size

### v1.2
- Optimized the hook installation flow
- Fixed an issue where the mode did not take effect after plugging in on some devices

## License

This project is released under the Mulan Public License, Version 2 (Mulan PubL v2). See [LICENSE](https://license.coscl.org.cn/MulanPubL-2.0) for the full text.

## Releases and Feedback

- Release page: https://github.com/Shuoh118/Auto-USB/releases
- Mirror release page: https://github.com/Xposed-Modules-Repo/io.github.shuoh118.autousbmtp/releases
- Issue tracker: https://github.com/Shuoh118/Auto-USB/issues

## Finally

- If you find this project useful, please hit the star in the top right corner. It means a lot to me.
- Thanks to @TigerSpirit217
- This project is based on https://github.com/TigerSpirit217/USBManager and modified from it. Without him, this project would not exist.

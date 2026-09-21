# Auto USB MTP

Xposed/LSPosed module: automatically switches the USB connection mode to MTP after the cable is plugged in, so you no longer have to pull down the notification shade and pick it manually every time.
-----
[中文](README.md)

## Function

- Automatically switches the USB mode to MTP after the data cable is plugged in
- Hooks UsbDeviceManager and AdbService, taking effect at the system_server layer

## Environmental requirements

- Android 12 and above (module minApiVersion / targetApiVersion = 102)
- LSPosed (Zygisk or Riru)
- Root access (KernelSU or Magisk)

## Install

1. Download the latest APK from Releases
2. Open the LSPosed manager after installation
3. Enable Auto USB MTP in the module list
4. Check the System Framework (system) scope
5. Reboot the device

## Configuration
Changes are written immediately and take effect the next time the cable is plugged in.

## Update Log

### v2.0
- Fixed the issue where rapid repeated plugging and unplugging of the cable was not detected
- Reduced the APK size

### v1.2
- Optimized the hook installation flow
- Fixed the issue where the mode did not take effect after plugging in on some models

## License

This project uses the Mulan Public License, version 2 (Mulan PubL v2). See LICENSE for the full text.

## Publish and Feedback

- Release page: github.com/Shuoh118/Auto-USB/releases
- Other release page: github.com/Xposed-Modules-Repo/io.github.shuoh118.autousbmtp/releases
- Issue feedback: github.com/Shuoh118/Auto-USB/issues

## At last

- If you find this project useful, please hit the star in the top right corner. It is the best encouragement for me.
- Thanks to @TigerSpirit217
- This project is based on github.com/TigerSpirit217/USBManager. Without him, this project would not exist.

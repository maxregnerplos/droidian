# Installation instructions

- [Installation instructions](#installation-instructions)
  - [Preparations](#preparations)
  - [Installation](#installation)
      - [Linux, Mac:](#linux-mac)
      - [Windows:](#windows)
  - [Finalizing installation](#finalizing-installation)

## Preparations

Ensure your device has a vendor partition from Android 10 (newer versions will not work). So, if you upgraded Android to newer version than Android 10 (Oreo), you have to downgrade Android first (flash Android 10).


Download the latest [nighly](https://github.com/miatoll-linux/droidian/releases/tag/nightly) release. It is recommended to ensure that you have the latest fastboot and adb versions.

## Installation

Unzip the downloaded zip archive, reboot your phone to fastboot (by pressing power and volume down buttons at the same time for a while) and connect the phone to your computer. Then, run following commands on your computer:

#### Linux, Mac:
* `chmod a+x ./flash_all.sh`
* `./flash_all.sh`
* _If the script above doesn't work you can use window's instructions below (remove .exe extension from the fastboot~~.exe~~ commands)_
#### Windows:

* `fastboot.exe flash boot data/boot.img`
* `fastboot.exe flash dtbo data/dtbo`
* `fastboot.exe flash userdata data/userdata.img`

## Finalizing installation

Now, you have to reboot the device. It should boot to phosh (a graphical user interface used by Droidian) after rebooting once more automatically. When the device has booted, you can unlock the device with the default passcode `1234`.

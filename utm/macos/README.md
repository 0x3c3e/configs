# UTM config to boot x86 macOS in QEMU

## Tested on
* Big Sur 11.7
* Monterey 12.6
* Ventura 13.3

## Dependencies
* [OpenCore](https://github.com/thenickdude/KVM-Opencore/releases/download/v20/OpenCore-v20.iso.gz)
* [UTM, Version 4.2.5](https://github.com/utmapp/UTM/releases/tag/v4.2.5)

## Troubleshooting
If keyboard/mouse don't work:
* turn on `Force PS/2 controller` option
* add `-global nec-usb-xhci.msi=off -usb -device usb-kbd -device usb-tablet`

## Supported CPUs
* Sandy Bridge
* Ivy Bridge

## Storage performance
* [raw](https://www.heiko-sieger.info/tuning-vm-disk-performance/) disk image

## macOS image
Download using [fetch-macOS-v2.py](https://github.com/kholia/OSX-KVM/blob/master/fetch-macOS-v2.py) script

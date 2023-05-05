# UTM config to boot x86 macOS in QEMU

## How to use?
* Create a new folder and name it with a `.utm` extension
* Place the provided [config.plist](https://github.com/0x3c3e/configs/blob/main/utm/macos/config.plist) file inside the folder
* Delete any existing drives in the UTM virtual machine
* Add the provided [OpenCore file](https://github.com/thenickdude/KVM-Opencore/releases/download/v20/OpenCore-v20.iso.gz) to the virtual machine
* Add a macOS installer to the virtual machine
* Add a blank disk to the virtual machine

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

## Get macOS image
* Download full installer using [installinstallmacos.py](https://github.com/munki/macadmin-scripts/blob/main/installinstallmacos.py) or [Makefile](https://github.com/thenickdude/OSX-KVM/blob/master/scripts/ventura/Makefile)
* Download recovery image using [fetch-macOS-v2.py](https://github.com/kholia/OSX-KVM/blob/master/fetch-macOS-v2.py) script (*slow*)

## Tested on
* Ventura 13.3.1

## Dependencies
* [OpenCore](https://github.com/thenickdude/KVM-Opencore/releases/download/v20/OpenCore-v20.iso.gz)
* [OVMF](https://www.kraxel.org/repos/jenkins/edk2/edk2.git-ovmf-x64-0-20220719.209.gf0064ac3af.EOL.no.nore.updates.noarch.rpm)

## Extract OVMF
```bash
tar -xf edk2.git-ovmf-x64-0-20220719.209.gf0064ac3af.EOL.no.nore.updates.noarch.rpm
mv usr/share/edk2.git/ovmf-x64/OVMF_CODE-pure-efi.fd OVMF.bin
```

## Storage performance
* [raw](https://www.heiko-sieger.info/tuning-vm-disk-performance/) disk image

## macOS image
Download using [fetch-macOS-v2.py](https://github.com/kholia/OSX-KVM/blob/master/fetch-macOS-v2.py) script
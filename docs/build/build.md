# How to Build UNISOC Zephyr SDK

### Choosing your board

The UNISOC Zephyr SDK supports building multiple boards.

### Choosing your profile

The UNISOC Zephyr SDK supports building multiple profiles.
All supported profiles are stored in the directory ```apps```,
and can be listed by the following command:

```shell
find apps/ -mindepth 1 -maxdepth 1 -type d ! -name ".*" -exec basename {} \;
```

### Building

To build a specific profile for a specific, use the following the command:

```shell
BOARD=96b_ivy5661 PROFILE=repeater make
```
Note that the default board is ```96b_ivy5661```, while the default profile is ```repeater```.

After the compilation, the images can be found in the directory ```output/repeater/images/```.

- fdl*.bin - Flash downloader
- mcuboot-pubkey*.bin - Bootloader
- zephyr-signed-ota*.bin - Kernel
- wcn-modem* - WCN Modem


# How to Build UNISOC Zephyr SDK

### **Downloading source code**
If you haven't installed ```repo``` yet, please install it first.
```shell
sudo apt-get install repo
```

To download the source code, please follow the commands below:

```shell
mkdir unisoc_zephyr_sdk && cd unisoc_zephyr_sdk
repo init -u https://github.com/unisoc/manifests.git -b master
repo sync
repo start --all master
```

### **Setting up Development Environment**
- [Install Requirements and Dependencies](https://docs.zephyrproject.org/latest/getting_started/installation_linux.html#install-requirements-and-dependencies)
- [Install Python Dependencies](https://docs.zephyrproject.org/latest/getting_started/getting_started.html#install-python-dependencies)
- [Install the Zephyr Software Development Kit](https://docs.zephyrproject.org/latest/getting_started/installation_linux.html#install-the-zephyr-software-development-kit-sdk)

For more information, please refer to [Getting Started Guide](https://docs.zephyrproject.org/latest/getting_started/getting_started.html#getting-started-guide).

### **Choosing your board**

The UNISOC Zephyr SDK supports building multiple boards.

- [96b_ivy5661](../boards/96b_ivy5661.md)

### **Choosing your profile**

The UNISOC Zephyr SDK supports building multiple profiles.
All supported profiles are stored in the directory ```apps```,
and can be listed by the following command:

- [repeater](../demos/wifi_repeater.md)

### **Building**

To build a specific profile for a specific board, use the following the command:

```shell
BOARD=96b_ivy5661 PROFILE=repeater make
```
Note that the default board is ```96b_ivy5661```, while the default profile is ```repeater```.

After the compilation, the images can be found in the directory ```output/repeater/images/```.

- fdl*.bin - Firmware downloader
- mcuboot-pubkey*.bin - Bootloader
- zephyr-signed-ota*.bin - Kernel
- wcn-modem* - WCN Modem


# How to Download UNISOC Zephyr SDK

To download the source code, please follow the commands below:

```shell
mkdir unisoc_zephyr_sdk && cd unisoc_zephyr_sdk
repo init -u https://github.com/unisoc/manifests.git -b master
repo sync
repo start --all master
```


# How to Set up Development Environment

## On Ubuntu install:
1) Install below tools
```shell
sudo apt-get install --no-install-recommends git cmake ninja-build gperf \
		 ccache dfu-util device-tree-compiler wget \
		 python3-pip python3-setuptools python3-wheel xz-utils file make gcc \
		 gcc-multilib
```
2) Install cmake version 3.8.2 or higher
```shell
wget https://cmake.org/files/v3.8/cmake-3.8.2-Linux-x86_64.sh
yes | sh cmake-3.8.2-Linux-x86_64.sh
sudo cp -r cmake-3.8.2-Linux-x86_64 /opt
```
3) Install Zephyr SDK 0.9.5 (default path: /opt/zephyr-sdk/)
```shell
wget https://github.com/zephyrproject-rtos/meta-zephyr-sdk/releases/download/0.9.5/zephyr-sdk-0.9.5-setup.run
sudo sh zephyr-sdk-0.9.5-setup.run
```

## Add zephyr env
Please refer to the below environment.
```shell
cat ~/.zephyrrc
export PATH=/opt/cmake-3.8.2-Linux-x86_64/bin:$PATH
export ZEPHYR_TOOLCHAIN_VARIANT=zephyr
export ZEPHYR_SDK_INSTALL_DIR=/opt/zephyr-sdk
export PATH=$ZEPHYR_SDK_INSTALL_DIR/sysroots/x86_64-pokysdk-linux/usr/bin/arm-zephyr-eabi:$PATH
```

## Reference
Please refer to [Getting Started Guide](https://docs.zephyrproject.org/latest/getting_started/getting_started.html#getting-started-guide).


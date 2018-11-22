# How to Set up Development Environment

## Precondition:
1. Install cmake-3.8.2-Linux-x86_64
2. Install zephyr-sdk-0.9.5

## Add zephyr environment
cat ~/.zephyrrc 
export PATH=/opt/cmake-3.8.2-Linux-x86_64/bin:$PATH
export ZEPHYR_TOOLCHAIN_VARIANT=zephyr
export ZEPHYR_SDK_INSTALL_DIR=/opt/zephyr-sdk
export PATH=$ZEPHYR_SDK_INSTALL_DIR/sysroots/x86_64-pokysdk-linux/usr/bin/arm-zephyr-eabi:$PATH

## Reference
Please refer to [Getting Started Guide](https://docs.zephyrproject.org/latest/getting_started/getting_started.html#getting-started-guide).


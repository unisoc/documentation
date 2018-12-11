# UNISOC Zephyr SDK

The UNISOC Zephyr SDK is provided for convenience and ease of use.
It provides everything you need for development of UNISOC hardware
platform except the cross-compilation toolchain, including
bootloader and Zephyr portings, top level customized applications
and programming tools.

### **Directory Structure**
- apps: contains example profiles.
- build: contains Makefiles and scripts that control the building process.
- dloader: is the firmware downloading tool running on PC.
- fdl: is the firmware downloading program running on the board.
- firmware: contains the WCN modem binary.
- mcuboot: contains the MCUboot source code.
- zephyr: contains the Zephyr source code.

### [Building UNISOC Zephyr SDK](build.md)

### [Updating Firmware](update_firmware.md)

### [Debugging](debug.md)


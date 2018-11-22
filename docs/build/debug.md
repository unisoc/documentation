# How to Debug

At present, debugging with the J-Link and GDB is the only choice.
To set the debugging environment, please follow the procedure below:

#### **Step 0**: Download [J-Link Software Pack](https://www.segger.com/downloads/jlink/JLink_Linux_V630b_x86_64.deb) and install it.

```shell
sudo dpkg -i Downloads/JLink_Linux_V630b_x86_64.deb
```

#### **Step 1**: Put Unisoc_UWP566X.JLinkScript to /opt/SEGGER/JLink/Samples/JLink/Scripts.

```shell
cp Unisoc_UWP566X.JLinkScript /opt/SEGGER/JLink/Samples/JLink/Scripts
```

#### **Step 2**: Start the J-Link GDB server

```shell
JLinkGDBServer -device Cortex-M4 -endian little -if SWD -speed 8000 -jlinkscriptfile /opt/SEGGER/JLink/Samples/JLink/Scripts/Unisoc_UWP566X.JLinkScript
```

#### **Step 3**: Start the debug session using GDB client


# uwpflash

### **WHAT IS THIS?**
DLoader is the firmware downloading tool for Unisoc MCU modules.

### **SOURCE CODE**

```shell
git clone https://github.com/unisoc/uwpflash.git
```

### **INSTALLATION**

```shell
make
sudo make install
```

### **USAGE**

It is able to update one or more images with one command:

```shell
uwpflash -t UART -d /dev/ttyUSB0 -f kernel.bin -a 0x2000000
```
or

```shell
uwpflash -t UART -d /dev/ttyUSB0 -f mcuboot.bin -a 0x2000000 -f signed-kernel.bin -a 0x2010000
```

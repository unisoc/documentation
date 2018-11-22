# DLoader

### **WHAT IS THIS?**
DLoader is the firmware downloading tool for Unisoc MCU modules.

### **SOURCE CODE**

```shell
git clone https://github.com/unisoc/dloader.git
```

### **INSTALLATION**

```shell
./configure
make
sudo make install
```

See the file INSTALL for compilation and installation instructions.


### **USAGE**
Please run `dloader` for a list and explanation of options.

However, it is recommended to use the wrapper script ```update_fw.sh```.

```shell
$ ./update_fw.sh -h
Usage: update_fw.sh [-d] path [-abhkmu]
-d: specify the path which contains images.
-a: flash all images.
-b: flash bootloader.
-k: flash kernel.
-m: flash modem.
-u: flash userdata
-h: display help.
```

# How to Update Firmware

To update firmware, please follow the procedure below:

#### **Step 0**: Install the flash programming tool before updating.
Download the [dloader](https://github.com/unisoc/dloader/releases/download/unisoc-v0.3.1/dloader_0.3.1-1_amd64.deb) and install it.

```shell
sudo dpkg -i dloader_0.x.x-1_amd64.deb
```

In addition, you can build the dloader.

```shell
make dloader
```

#### **Step 1**: Switch bootstrap pin to ```Download``` mode.
![Download Mode](/extras/images/download_mode.png)

#### **Step 2**: Power on the board, and check the name of your serial port.
```shell
$ dmesg | tail
[18063.042470] usb 1-1.4: new full-speed USB device number 10 using ehci-pci
[18063.137325] usb 1-1.4: New USB device found, idVendor=10c4, idProduct=ea60
[18063.137332] usb 1-1.4: New USB device strings: Mfr=1, Product=2, SerialNumber=3
[18063.137335] usb 1-1.4: Product: CP2104 USB to UART Bridge Controller
[18063.137338] usb 1-1.4: Manufacturer: Silicon Labs
[18063.137341] usb 1-1.4: SerialNumber: 018B5764
[18063.138117] cp210x 1-1.4:1.0: cp210x converter detected
[18063.210553] usb 1-1.4: reset full-speed USB device number 10 using ehci-pci
[18063.303396] usb 1-1.4: cp210x converter now attached to ttyUSB0
```

#### **Step 3**: Updating firmware by the following commands.

```shell
cd output/repeater/images
./update_fw.sh
```
Note that the default serial port name is ```ttyUSB0```.
Otherwise, you should specify the serial port name got from **Step 2**.

```shell
cd output/repeater/images
./update_fw.sh -d ttyUSB0
```

#### **Step 4**: Switch bootstrap pin to ```Boot``` mode again and push the reset button.
![Boot Mode](/extras/images/boot_mode.png)

To update one image or several images, please refer to help of ```update_fw.sh```.

```shell
./update_fw.sh -h
```


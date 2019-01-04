# Wi-Fi Repeater User Guide

To make the Wi-Fi repeater work, please follow the procedure below:

### **0. Install Smart Repeater to your phone.**
Download the [Smart Repeater](https://github.com/unisoc/Android-SmartRepeater/releases/download/W19.01.05/SmartRepeater_W19.01.05.apk).

Connect your phone to the PC, and use the following command to install it.

```shell
adb install smartRepeater_Wxx.xx.x.apk
```

### **1. Power on the board by connect UART0 to your PC/AC adapter.**
![Power On](/extras/images/power_on.png)

### **2: Open Smart Repeater and connect to the board through BLE.**
Tap the ```scan``` button.

![BLE 0](/extras/images/smartrepeater_ble_0.png)

Choose ```uwp566X_XXXX```, and wait for the connection.

![BLE 1](/extras/images/smartrepeater_ble_1.png)
![BLE 2](/extras/images/smartrepeater_ble_2.png)

### **3. Configure Wi-Fi Station by Smart Repeater.**
Tap the ```menu``` button, and choose ```WiFi Manager```.

![STA 0](/extras/images/smartrepeater_sta_0.png)
![STA 1](/extras/images/smartrepeater_sta_1.png)

Tap ```OPEN WIFI```.

![STA 2](/extras/images/smartrepeater_sta_2.png)

Tap ```WIFI SCAN```, and wait for the scanning.

![STA 3](/extras/images/smartrepeater_sta_3.png)
![STA 4](/extras/images/smartrepeater_sta_4.png)

Tap the drop-down menu, and select the target router.

![STA 5](/extras/images/smartrepeater_sta_5.png)
![STA 6](/extras/images/smartrepeater_sta_6.png)

Enter the password.

![STA 7](/extras/images/smartrepeater_sta_7.png)

Tap ```CONNECT```, and wait for the connection.

![STA 8](/extras/images/smartrepeater_sta_8.png)
![STA 9](/extras/images/smartrepeater_sta_9.png)

### **4. Configure Wi-Fi AP by Smart Repeater.**

After the connection is completed, tap ```START AP```.

![AP 0](/extras/images/smartrepeater_ap_0.png)
![AP 1](/extras/images/smartrepeater_ap_1.png)

At last, Remember the AP’s ```MAC```.

![AP 2](/extras/images/smartrepeater_ap_2.png)

### **Note:**

- STA should be connected before starting AP. 
- When STA is connected to any AP, the green light will be turned on.
- When AP is started, the blue light will be turned on.
- When both green and blue light are turned on, the Wi-Fi repeater is ready to work.
- The repeater's SSID is ```UNISOC_XXXXXX``` by default, while ```XXXXXX``` is the NIC of AP’s MAC.
- The repeater's password is the same as the router's by default.

Now you can connect your phone to the repeater, and open any website in the browser to check whether the repeater works.


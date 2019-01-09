# zperf

### **WHAT IS THIS?**
zperf is a network traffic generator for Zephyr that may be used to evaluate network bandwidth.

### **SOURCE CODE**

```shell
git clone https://github.com/unisoc/apps.git
cd apps/zperf
```

### **BUILD**
1)Please setup environment as the below URL.
- [Build UNISOC SDK](../sdk/build.md)

2)Specifi the PROFILE to zperf
```shell
PROFILE=zperf make
```
3)See the build result and check if binaries generated.

```shell
cd output/zperf/images
```

### **UPDATE FIRMWARE**
Please update firmware as the below URL.
- [Update firmware](../sdk/update_firmware.md)


### **USAGE**
- [Zephyr zperf guide](http://docs.zephyrproject.org/latest/samples/net/zperf/README.html)

Here are examples.

UDP RX:
1) Run on board
```shell
uart:~$ zperf udp download 5001
```
2) Run on PC
```shell
iperf -l 1K -c 192.168.20.127 -p 5001 -i 1 -u
```

UDP TX:
1) Run on PC
```shell
iperf -s -l 1K -u -B 192.168.1.142
```
2) Run on board
```shell
uart:~$ zperf udp upload 192.168.1.142 5001 10 1K 100M
```

TCP RX:
1) Run on board
```shell
uart:~$ zperf tcp download 5001
```
2) Run on PC
```shell
iperf -l 1K -c 192.168.20.127 -p 5001 -i 1
```

TCP TX:
1) Run on PC
```shell
iperf -s -l 1K -B 192.168.1.142
```
2) Run on board
```shell
uart:~$ zperf tcp upload 192.168.1.142 5001 10 1K 100M
```


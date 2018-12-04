# Releases

## v0.3.3

###	Major enhancements with this release
- WIFIMGR: Use work queue to offload event timeout handling.
- SIPC: Disable IRQ relay for some WIFI interrupts which are polled by CP.
- Flash: Support flash page layout.
- IWNPI: Implement hw_test interface to mp test.
- Zephyr: Enable NEWLIBC to support more features.
- FDL: Refactor fdl to use UART interrupt instead of polling.
- Various bugs fix.

###	Commits
#### Application
- 2018-12-04 11:22:01 +0800-4128b15-Dong Xiang: repeater: Enable NEWLIBC.
- 2018-12-04 11:22:01 +0800-4fb4ab2-Dong Xiang: Repeater: Enable ASSERT to get more messages when crashed.
- 2018-12-03 10:05:41 +0800-e576de9-Jessie.Xin: mp_test: iwnpi: add support to driver new api of hw_test
- 2018-12-03 09:53:18 +0800-37a41a2-ling.zhou: mesh_light: Remove unused ipi configuration Remove unused ipi configuration leading to a compile error
#### Build
- 2018-11-29 16:46:51 +0800-964e890-Keguang Zhang: update_fw.sh: update the wrapper script of dloader
- 2018-11-28 18:51:50 +0800-4a3c0fa-Keguang Zhang: root.mk: Update Makefile to support fdl
#### Firmware
- 2018-12-04 17:32:01 +0800-5f66a83-Keguang Zhang: Update WCN modem binary
- 2018-11-29 10:59:41 +0800-dac1e50-Dong Xiang: wifi: disable BB_TS_INT interrupt by firmware.
#### Zephyr
- 2018-12-03 19:11:09 +0800-2e8f573-Stephen.Zhang: drivers: flash: Adapt uwp configs to call setting subsys.
- 2018-12-03 11:03:48 +0800-2b894c0-Jessie.Xin: include: net: fix build warning in wifi_drv_api
- 2018-12-03 10:30:02 +0800-ce984db-Keguang Zhang: subsys: wifi: use workqueue to offload event timeout handling
- 2018-11-30 18:39:02 +0800-20de07c-Keguang Zhang: subsys: wifi: improve WiFi manager
- 2018-11-30 15:51:49 +0800-ca0e607-Bub Wei: drivers: wifi: Implement hw_test api
- 2018-11-30 15:48:28 +0800-32b5989-Jessie.Xin: include: net: add new wifi driver api for hw_test
#### HAL
- 2018-12-04 15:26:28 +0800-7cf5027-Dong Xiang: drivers: sipc: Enable NVIC_INT_REQ_COM_TMR relay to avoid wifi scan issue.
- 2018-12-03 19:13:47 +0800-34f5e48-Stephen.Zhang: drivers: sfc: Code implements for lock/unlock api on xip.
- 2018-11-29 11:02:38 +0800-9b01b4a-Dong Xiang: drivers: sipc: Disable all WIFI irq relay.

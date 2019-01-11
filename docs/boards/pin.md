
#pin on the female header

PLACE | NAME | FUNCTION DECLARATION  | DIRECTION | PORT | PIN | DEFAULT
-- | ------ | ---------------- | -- | --| - | -
1 | GND | connect to GND | - | - | - | -
2 | GND | connect to GND | - | - | - | -
3 | U1CTS | 0: U1CTS<br>3: GPIO24<br>5: PCIe_DBG11 | I<br>I/O/T<br/>O | 1 | 8 | FUNC0
4 | PWR_BTN_N | external access; <br>control power supply of board. | - | - | - | -
5 | U1TXD | 0: U1TXD<br>3: GPIO21<br>5: PCIe_DBG8 | O<br>I/O/T<br>O | 1 | 5 | FUNC0 
6 | RST_N | reset board | I | - | - | -
7 | U1RXD | 0: U1RXD<br>3: GPIO22<br>5: PCIe_DBG9 | I<br>I/O/T<br>O | 1 | 6 | FUNC0
8 | SD_CLK | 0: SD_CLK<br>3: GPIO19<br>5: PCIe_DBG4 | I/O/T<br>I/O/T<br>O | 1 | 3 | FUNC0
9 | U1RTS | 0: U1RTS<br>3: GPIO23<br>5: PCIe_DBG10 | O<br>I/O/T<br>O | 1 | 7 | FUNC0
10 | SD_D0 | 0: SD_D0<br>3: GPIO18<br>5: PCIe_DBG3 | I/O/T<br>I/O/T<br>O | 1 | 2 | FUNC0
11 | U2TXD | 0: PCIE_WAKE_L<br>1: U2TXD(G1)<br>3: GPIO42 | I/O/T<br>O<br>I/O/T | 2 | 10 | FUNC0
12 | SD_CMD | 0: SD_CMD<br>3: GPIO20<br>4: DB7(G1)<br>5: PCIe_DBG5 | I/O/T<br>I/O/T<br>O<br>O | 1 | 4 | FUNC0
13 | U2RXD | 0: PCIE_RST_L<br>1: U2RXD(G1)<br>3: GPIO41 | I<br>I<br>I/O/T | 2 | 9 | FUNC0
14 | SD_D1 | 0: SD_D1<br>3: GPIO17<br>5: PCIe_DBG2 | I/O/T<br>I/O/T<br>O | 1 | 1 | FUNC0
15 | I2CSCL | 0: U3RXD<br>1: I2C_SCL<br>3: GPIO31<br>5: PCIe_DBG7 | I<br>I/O/T<br>I/O/T<br>O | 1 | 15 | FUNC0
16 | IISRCK | 0: IISLRCK<br>1: IIS1LRCK<br>2: COEX5<br>3: GPIO6<br>4: DB2(G0)<br>5: WB11 | I/O/T<br>I/O/T<br>I/O<br>I/O/T<br>O<br>O | 0 | 6 | FUNC0
17 | I2CSDA | 0: U3TXD<br>1: I2C_SDA<br>3: GPIO30<br>5: PCIe_DBG6 | O<br>I/O/T<br>I/O/T<br>O | 1 | 14 | FUNC0
18 | IISCLK | 0: IISCLK<br>1: IIS1CK<br>2: COEX4<br>3: GPIO5<br>4: DB1(G0)<br>5: WB10 | I/O/T<br>I/O/T<br>I/O<br>I/O/T<br>O<br>O | 0 | 5 | FUNC0
20 | IISDO | 0: IISDO<br>1: IIS1DO<br>2: COEX3<br>3: GPIO4<br>4: DB0(G0)<br>5: WB9 | O/T<br>O/T<br>I/O<br>I/O/T<br>O<br>O | 0 | 4 | FUNC0
22 | IISDI | 0: IISDI<br>2: COEX6<br>3: GPIO7<br>4: DB3(G0)<br>5: WB12 | I<br>I/O<br>I/O/T<br>O<br>O | 0 | 7 | FUNC0
23 | INT | 0: INT<br>2: COEX7<br>3: GPIO10 | O<br>I/O<br>I/O/T | 0 | 10 | FUNC0
24 | GPIO25 | 0: GNSS_LNA_EN<br>2: FDMA_CEN<br>3: GPIO25 | O<br>I<br>I/O/T | 1 | 9 | FUNC3
25 | WCI_2_TXD | 0: WCI_2_TXD<br>2: COEX1<br>3: GPIO9<br>4: DB7(G0)<br>5: WB4 | O<br>I/O<br>I/O/T<br>O<br>O | 0 | 9 | FUNC0
26 | WCI_2_RXD | 0: WCI_2_RXD<br>2: COEX0<br>3: GPIO8<br>4: DB2(G1)<br>5: WB3 | I<br>I/O<br>I/O/T<br>O<br>O | 0 | 8 | FUNC0
27 | RFCTL0 | 0: RFCTL0<br>2: SOC_DBG0<br>3: GPIO32<br>5: WB13 | O<br>O<br>I/O/T<br>O | 2 | 0 | FUNC3
28 | GPIO43 | 0: U0TXD<br>3: GPIO43<br>5: PCIe_DBG12 | O<br>I/O/T<br>O | 2 | 11 | FUNC0
29 | RFCTL1 | 0: RFCTL1<br>2: SOC_DBG1<br>3: GPIO33<br>5: WB14 | O<br>O<br>I/O/T<br>O | 1 | 1 | FUNC3
30 | RFCTL3 | 0: RFCTL3<br>2: SOC_DBG3<br>3: GPIO35<br>5: WB16 | O<br>O<br>I/O/T<br>O | 1 | 3 | FUNC3
31 | RFCTL2 | 0: RFCTL2<br>2: SOC_DBG2<br>3: GPIO34<br>5: WB15 | O<br>O<br>I/O/T<br>O | 1 | 2 | FUNC3
32 | RFCTL4 | 0: RFCTL4<br>2: SOC_DBG4<br>3: GPIO36<br>5: WB17 | O<br>O<br>I/O/T<br>O | 1 | 4 | FUNC3
33 | MTMS | 0: MTMS<br>1: PPS(G0)<br>2: FDMA_MISO<br>3: GPIO11<br>4: DB0(G1)<br>5: WB5 | I/O<br>O<br>O<br>I/O/T<br>O<br>O | 0 | 11 | FUNC0
34 | MTCK | 0: MTCK<br>1: T_DIG(G0)<br>2: FDMA_MOSI<br>3: GPIO12<br>4: DB1(G1)<br>5: WB6 | I<br>I<br>I<br>I/O/T<br>O<br>O | 0 | 12 | FUNC0
35 | VDD1V8 | connect to 1.8V VDD | - | - | - | -
37 | USB_VBUS | connect to USB to provide power | - | - | - | -
39 | GND | connect to GND | - | - | - | -
40 | GND | connect to GND | - | - | - | -


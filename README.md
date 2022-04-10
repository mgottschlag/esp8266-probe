# esp8266-probe

This repository contains a PCB design for a WIFI JTAG probe using the ESP-12
ESP8266 module. The probe is designed to be compatible with
[blackmagic-espidf](https://github.com/walmis/blackmagic-espidf). The JTAG
signals (+UART) are connected as follows to ESP8266 GPIOs:

| JTAG Signal | GPIO |
| ----------- | ---- |
| TXD         | 1    |
| RXD         | 3    |
| TMS/SWDIO   | 4    |
| TCK/SWCLK   | 5    |
| SRST        | 12   |
| TDI         | 13   |
| TDO         | 14   |

In addition, the 10-pin connector provides 5V and 3.3V supplies. The PCB is
provided with power via USB and 3.3V is provided by a cheap 1117 linear
regulator.

## License

The design is licensed under the [CERN Open Hardware Licence Version 2 - Permissive](cern-ohl_p_v2.txt).

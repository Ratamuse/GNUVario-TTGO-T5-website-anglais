---
step: 1
description: Hardware configuration
---

This part is only necessary if you want to use non-standard equipment to make your GnuVario-E

Before configuring the hardware part, you must know how to [compile the code]({{site.baseurl}}{% link 5-code.md%}). Make sure you know the Arduino IDE.

The configuration linked to the hardware is done by editing the files [libraries/HardwareConfig/HardwareConfig.h](https://github.com/prunkdump/GNUVario-TTGO-T5/tree/master/Sources/Beta%20Code/libraries/HardwareConfig/HardwareConfig.h) and [libraries/HardwareConfig/HardwareConfigESP32.h](https://github.com/prunkdump/GNUVario-TTGO-T5/tree/master/Sources/Beta%20Code/libraries/HardwareConfig/HardwareConfigESP32.h) in your Arduino folder. If you do not have an editor suitable for writing code, you can download it [Notepad ++](https://notepad-plus-plus.org/).

Start by checking the files. There is a file common to all the microcontrollers and a file linked to the ESP32 (TTGO-T5). The configuration of the **hardware**, number of pins, addresses of cards or memory are in these files. Each option is documented by comments directly inside this file, read them carefully.

To "comment" a line add "//" at the beginning. This disables the option.

Normally, if you are using a screen other than 1.54 "in size, you should only have to adapt the screen type: this is the **VARIOSCREEN_SIZE** directive in the HardwareConfig.h file.


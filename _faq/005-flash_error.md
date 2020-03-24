---
description: Error during flashing
---

- Start the vario with the switch, before connecting it to the PC via the USB socket, then start the compilation / flashing operation.
- If this does not work: start the vario just when flashing will start, whether with the Arduino IDE, the PlatformIO IDE, or the 'Flash tools'.

For example, with the **IDE Arduino**:
wait for the line "Linking everything together ...", then switch on the vario.
It is even possible to wait for the message "the selected serial port does not exist or your Arduino is not connected _____....._____....." to turn on the vario.

another example, with **PlatformIO**:
wait for the line "Linking .pio \ build \ esp32dev \ firmware.elf", then switch on the vario.
It is even possible to wait for the message "Connecting ........_____....._" to switch on the vario.

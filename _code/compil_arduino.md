---
step: 4
description: Compiling with Arduino IDE 
---

Compile the code
-----------------
Beforehand, you must start the vario without the sdcard, **then** connect it to the PC via the USB socket. It will be recognized by the PC as a COMx serial interface (example: COM4).

Now launch the Arduino IDE and open the sketch you want to compile. For example, the sketch **Gnuvario-E.ino**.

![GitHub download zip]({{"/assets/code_img/code5.jpg" | absolute_url}})

In the **Tools** menu, **make sure you choose the right card**. The most classic of this project is the **ESP32 Dev Module**.

and select partition scheme: **Minimal SPIFFS (1.9 MB APP with OTA / 180 KB SPIFFS)**

Still in the **Tools** menu, choose the serial port corresponding to the vario.

![GitHub download zip]({{"/assets/code_img/ide1.jpg" | absolute_url}})

Just click the **upload** button.

![GitHub download zip]({{"/assets/code_img/code7.jpg" | absolute_url}})

This will launch the compilation of the code, then update the vario; the vario will restart alone at the end of the procedure.

You can now disconnect the USB output, stop the vario, insert the sdcard and start it again.




---
description: Error compiling the code in the Arduino IDE
---

- The default Arduino folder (under Windows,*Documents / Arduino*) must contain only the Gnuvario project files; in fact, two files:
  - *Gnuvario-E*: contains Gnuvario-E.ino
  - *libraries*: the project libraries, and only these.
- You must start the vario with the switch and without the sdcard, before connecting it to the PC via USB.
- In the menu *Tools* of the Arduino IDE, the chosen card must be *ESP32 Dev Module*, the partition scheme *Minimal SPIFFS (1.9 MB APP with OTA / 180 KB SPIFFS)*, and the COM port that corresponding to vario.


See [the dedicated documentation]({{ site.baseurl }}/5-code.html)
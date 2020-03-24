---
step: 3
title: Manual
description: First start
---

Before you can use Gnuvario-E you must install the software and prepare the SD card

### Preparing the SD card #
On a blank MicroSD card formatted in Fat16 or 32, copy the contents of the RootSD folder to the root of the SD card.

### Update of Gnuvario-E #
Before updating the vario you must download and install the flash download tools from express

Flash Download Tools: <https://www.espressif.com/en/support/download/other-tools>

Start the Gnuvario-E without the SD card; ** then ** connect it to the PC by the usb port. The PC will see the vario as a serial port; for example, COM3.

Run flash_download_tools.exe; choose the option 'ESP32 DownloadTool'.

Then choose the last .bin file, using the following parameters (choose the COM port corresponding to the vario):

![Flash_download_tools]({{'/assets/manuel_img/flashTools.jpg' | relative_url}})

Press the Start button; the green square 'IDLE' then indicates 'Download', and a green progress bar is displayed at the bottom of the utility.
Writing the software takes about 2 minutes; when finished, the green square displays 'FINISH'.

You can then cut the power to the Gnuvario-E, disconnect the usb port, insert the sdcard and restart the vario.
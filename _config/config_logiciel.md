---
step: 2
description: Software configuration
---

There are 3 methods to configure your variometer with your personal parameters

**a) The web page**

The easiest way to configure your GnuVario-E is to use the on-board web page and Wifi mode.
This will automatically update the configuration files on the sdcard.
This functionality is described in the [user manual]({{site.baseurl}}{% link 7-manuel.md%}).

**b) Configuration files on the SD card**

These files are located at the root of the SD card; they are described in more detail at the bottom of this page.
They allow you to configure the GNUVario without having to recompile the code.
- params.jso: contains the general parameters of the GNUVario.
- wifi.cfg: contains the connection information to the wifi network; you can declare up to 4 different wifi networks.
- variocal.cfg: contains the GNUVario calibration information. See the [user manual]({{site.baseurl}}{% link 7-manuel.md%}) for the calibration operation.

**c) The VarioSettings.h file**

This method is reserved for experienced users who wish to use non-standard material or recompile the code.

If you do not want to use an SD card, you can modify the libraries / VarioSettings / VarioSettings.h file to customize your vario. Using this file requires recompiling the code.

[libraries/VarioSettings/VarioSettings.h](https://github.com/prunkdump/GNUVario-TTGO-T5/tree/master/Sources/Beta%20Code/libraries/VarioSettings/VarioSettings.h)

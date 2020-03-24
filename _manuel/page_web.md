---
step: 5
title: Manual
description: Web page
---

The GnuVario-E embeds a Web server; it is accessed after the wifi connection, via a web browser. See previous page of the manual.

The home page looks like this:
{%include manuelimg.md name="pageweb_01.jpg"%}

or like this, if the screen width does not allow the display of all the menus.
{%include manuelimg.md name="pageweb_02.jpg"%}

In the latter case, simply click on the menu icon, at the top right, to access the menu.

The different menu options are described now.

### "My flights" menu

This is the menu proposed by default. It lists the different IGC files of the flights saved on the SD card.
For each flight, you can:
- delete the recording
- download it
- view it briefly



### "SD card" 

Presents the contents of the SD card. Allows you to create / delete folders, download or upload files.
{%include manuelimg.md name="SDcard_01.jpg"%}
#### Folders
The files are proposed first. If you click on the title of a folder, you open it, and the included files are displayed; we see it in the previous screenshot, for the 'flights' folder.
New files can be placed in a folder by clicking on the blue 'Download' icon; you can also delete a folder and all the files included by clicking on the red 'Delete' icon.
#### Files
The file can be downloaded to the computer by clicking on the green 'Download' icon; you can also delete the file by clicking on the red 'Delete' icon.

### "Wifi" 

Allows you to specify the wifi networks to which the vario can potentially connect.
It is possible to declare up to 4 wifi networks.
The result is written on the SD card, in the file '/wifi.cfg'

### "Configuration" 

The options offered in this tab allow you to customize the operation of the vario; they are linked to the file '/params.jso' on the SD card.
The parameters are described in the ['Configuration']({{site.baseurl}}/6-configuration.html) part of the GNUVario documentation.

These parameters are divided into 4 tabs:
'_Général_' - '_Vario_' - '_Start of the flight_' - '_System_'
{%include manuelimg.md name="configuration_01.jpg"%}
- General
Used to describe the sails or sails on which we are flying, and the name of the pilot.
Mainly used for UGC flight recordings
- Vario
Allows you to configure the operation of the vario: threshold for triggering beeps, and different options
- Flight start
Defines the criteria that will allow the vario to determine that a flight has just started.
- System
Allows you to adjust various parameters relating to the operation of the vario: beeps when starting the vario, the flight, the fixed GPS, activation of flight recording, temperature compensation or GPS altitude, ...

### "Update" 
Used to update the vario software.
{%include manuelimg.md name="update_01.jpg"%}
The update can be done 'locally', from a computer that has a desired firmware version.

It is also possible to automatically update the firmware from the web.

See the documentation dedicated to updating the vario.
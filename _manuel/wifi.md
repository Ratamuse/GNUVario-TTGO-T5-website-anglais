---
step: 4
title: Manual
description: Wifi
---

The Gnuvario-E has a web server, which will allow you to configure the Gnuvario, update it,
  recover flight files but also copy or recover files on the SDCard
 
{% include manuelimg.md name = "ecran291wifireboot.png"%}

**WiFi settings**

Before you can use Wifi with the Gnuvario-E, you must indicate the SSID and password of your Box or your phone

Complete the information in the wifi.cfg file. You can specify up to 4 different WiFi networks.

If you do not want to use the SD card, you will have to complete the variosettings.h file (requires compilation of the code).


#define DEFAULT_VARIOMETER_SSID_1													"your_SSID1"   
#define DEFAULT_VARIOMETER_PASSWORD_1											"your_PASSWORD_for SSID1"   

#define DEFAULT_VARIOMETER_SSID_2													"your_SSID2"   
#define DEFAULT_VARIOMETER_PASSWORD_2											"your_PASSWORD_for SSID2"   

#define DEFAULT_VARIOMETER_SSID_3													"your_SSID3"   
#define DEFAULT_VARIOMETER_PASSWORD_3											"your_PASSWORD_for SSID3"   

#define DEFAULT_VARIOMETER_SSID_4													"your_SSID4"   
#define DEFAULT_VARIOMETER_PASSWORD_4											"your_PASSWORD_for SSID4"   

**Switching to Wifi mode**

At startup, press the left button

As soon as the Gnuvario-E is connected to the Wifi network, the address of the web page is displayed on the screen:



**Connection to the web page**

In your web browser, login with the IP address provided.





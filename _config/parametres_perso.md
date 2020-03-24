---
step: 3
description: List of customizable parameters
---

### params.jso #

It is a file in json format, which allows you to customize the operation of GnuVario.

The main parameters of this file are:

**system - SLEEP_TIMEOUT_MINUTES**

default: 20 minutes
standby after X minutes of inactivity

**system - SLEEP_THRESHOLD_CPS**

default: 0.5 m
activity trigger threshold (equivalent to +0.5 Vz)

**system - ALARM_SDCARD**

1 = Alarm beep indicating that the SD card is not present

**system - ALARM_GPSFIX**

1 = Beep indicating that the GPS is operational

**system - ALARM_FLYBEGIN**

1 = Beep indicating the start of flight recording

**system - NO_RECORD**

default: 0
1 = deactivation of recording on the SDcard

**system - BT_ENABLE**

default: 0
1 = Bluetooth enabled

**system - COMPENSATION_TEMP**

default: -6
temperature compensation

**system - COMPENSATION_GPSALTI**

default: -30
Gps altitude compensation

**system - MULTIDISPLAY_DURATION**

default: 2000 milliseconds
Display time of the different pages (in milliseconds)

**system - DEFAULT_DISPLAY_STAT_DURATION**

default: 6
time in sec display of the statistics screen at startup

**system - URL_UPDATE**

default: http://gnuvario-e.yj.fr/update/firmware.json
Path to update storage site

**general - TIME_ZONE**

Defines the UTC time zone: (+2) in summer (+1) in winter

**general - PILOT_NAME**

Pilot name

**general - GLIDER_NAMEx**

x from 1 to 4: Allows you to enter 4 names of wing

**general - GLIDER_SELECT**

Allows you to choose 1 wing, among the 4 possible

**vario - SINKING_THRESHOLD**

default: -2.0
Triggering threshold

**vario - CLIMBING_THRESHOLD**

default: 0.2
Zeroing trigger threshold

**vario - NEAR_CLIMBING_SENSITIVITY**

default: 0.5
Zero zone

from -10 to -2.0 low gross sound
from -2.0 to 0.2 no sound
from 0.2 to 0.5 zero beep
0.5 to 10 rise beeps

**vario - ENABLE_NEAR_CLIMBING_ALARM**

default: 0
1 = Near climb alarm: signals that you are entering or leaving the near climb zone

**vario - ENABLE_NEAR_CLIMBING_BEEP**

default: 0
1 = Zero beep: beep when you are in an area between VARIOMETER_CLIMBING_THRESHOLD and VARIOMETER_NEAR_CLIMBING_SENSITIVITY

**vario - DISPLAY_INTEGRATED_CLIMB_RATE**

default: 0
1 = Display of the average fall rate over a period
0 = Display of instantaneous fall rate

**vario - CLIMB_PERIOD_COUNT**

default: 10
integration time for calculating the sink rate

**vario - SETTINGS_GLIDE_RATIO_PERIOD_COUNT**

default: 20
drop rate display frequency

**vario - RATIO_CLIMB_RATE**

default: 2
1 = Display of the fineness
2 = Display of the average fall rate
3 = Display of the 2 information alternately in the area to the right of the vario poster

**vario - RATIO_MAX_VALUE**

default: 30.0
max value used in calculating the sink rate

**vario - RATIO_MIN_SPEED**

default: 10.0
minimum speed value used in calculating the fall rate

**vario - SENT_LXNAV_SENTENCE**

default: 1
BT transmission format
1 = LXNAV
0 = LK8000

**flightstart - FLIGHT_START_MIN_TIMESTAMP**

default: 15000 milliseconds
Minimum time between flight start and start in milliseconds

**flightstart - FLIGHT_START_VARIO_LOW_THRESHOLD**

default: 0.5
**flightstart - FLIGHT_START_VARIO_HIGH_THRESHOLD**

default: 0.5
Minimum vertical speed in m / s (low / high threshold) to trigger recording

**flightstart - FLIGHT_START_MIN_SPEED**

default: 8 km / h
Minimum ground speed in km / h triggering flight recording

**flightstart - VARIOMETER_RECORD_WHEN_FLIGHT_START**

default: 1
0 = deactivated, recording starts as soon as the GPS is operational
1 = Activated, recording will start upon detection of the start of flight (horizontal speed greater than FLIGHT_START_MIN_SPEED and horizontal speed less than FLIGHT_START_VARIO_LOW_THRESHOLD or greater than FLIGHT_START_VARIO_HIGH_THRESHOLD

### wifi.cfg #

This file contains the wifi connection parameters.
You can configure up to 4 wifi networks

**SSID_1**

default: your_SSID1
SSID of the first Wifi network

**PASSWORD_1**

default: your_PASSWORD_for SSID1
Password of the first Wifi network

**SSID_2**
**PASSWORD_2**


**SSID_3**
**PASSWORD_3**


**SSID_4**
**PASSWORD_4**

### variocal.cfg #

This file contains the GNUVario calibration values.

**VERTACCEL_GYRO_CAL_BIAS_00**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_01**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_02**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_03**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_04**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_05**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_06**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_07**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_08**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_09**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_10**

default: 0x00

**VERTACCEL_GYRO_CAL_BIAS_11**

default: 0x00

**VERTACCEL_ACCEL_CAL_BIAS_00**

default: 0x00

**VERTACCEL_ACCEL_CAL_BIAS_01**

default: 0x00

**VERTACCEL_ACCEL_CAL_BIAS_02**

default: 0x00

**VERTACCEL_ACCEL_CAL_SCALE**

default: 0

**VERTACCEL_MAG_CAL_BIAS_00**

default: 0

**VERTACCEL_MAG_CAL_BIAS_01**

default: 0

**VERTACCEL_MAG_CAL_BIAS_02**

default: 0

**VERTACCEL_MAG_CAL_PROJ_SCALE**

default: 15535

**VERTACCEL_ACCEL_CAL_BIAS_MULTIPLIER**

default: 5

**VERTACCEL_MAG_CAL_BIAS_MULTIPLIER**

default: 5



### log.cfg #

This file contains the debugging configuration values.

**LOG_ENABLE**

default: 1
Debugger activation
     
**LOG_SERIAL_ENABLE**

default: 1
Activation of messages on the serial port
     
**LOG_SD_ENABLE**

default: 1
Activation of messages on the SdCard
      
**LOG_DEBUG_ENABLE**

default: 1
Activation of messages in ESP32 debug mode

**MAIN_DEBUG**

default: 0
Activation of main program messages

**SCREEN_DEBUG**

default: 0
Activation of messages concerning screen management

**GPS_DEBUG**

Default: 0
Activation of messages concerning GPS

**BUTTON_DEBUG**

Default = 0
Activation of messages concerning button management

**MS5611_DEBUG**

Default: 0
Activation of messages concerning the barometric sensor

**MPU_DEBUG**

Default: 0
Activation of messages concerning accelerometers, gyroscope, ...
 
**SDCARD_DEBUG**

Default: 0
Activation of messages concerning the SD card

**BT_DEBUG**

Default: 0
Activation of messages concerning Bluetooth

**WIFI_DEBUG**

Default: 0
Activation of messages concerning WiFi

**SOUND_DEBUG**

Default: 0
Sound messages activation

**DEEPSLEEP_DEBUG**

Default: 1
Activation of messages concerning standby mode  




---
step: 7
title: Manual
description: Calibration
---

**It is important to calibrate the accelerometers**

The GnuVario-E incorporates an accelerometer, which must be calibrated.

First on Windows or Mac, install [Python version 2](https://www.python.org/). On Windows, be sure to check the option **add to PATH variable**.
       
Retrieve the code {% include lienfichier.md name = "calibration.zip" lien = "file / calibration.zip"%} which you will place in a folder named for example "calibration"
      
Copy the {% include lienfichier.md name = "variocal.cfg" lien = "file / variocal.cfg"%} file on the SD card
       
Make sure your SD card is inside the variometer.
         
Turn on the Gnuvario-E
Enter calibration mode by pressing the right button at startup (at the init screen).
You have a few seconds to place the vario flat and press the central button.

**Wait for the 3 beeps** then start to rotate the vario in all directions
You must make approximately 5 to 6 movements per side while waiting for the beep between each movement
The more measurements you make, the more precise the calibration.

**WARNING it is essential not to forget any side**

At the end, press the left button of the vario to complete the calibration. The vario restarts.

<iframe width = "560" height = "315" src = "https://www.youtube.com/embed/6yxoZcxxzVY" frameborder = "0" allow = "autoplay; encrypted-media" allowfullscreen> </iframe>

This will create a "RECORD **. CAL" file on the SD card. Copy this file to the "best-fit-calibration" folder and rename it if necessary as "RECORD00.IGC".

Under Windows or Mac, launch the **Idle** Python and open the program "calibrage / calibrer.py". Press "F5" to execute.
    
{%include manuelimg.md name="python_file.jpg"%}

or
      
{% highlight shell_session%}
c:> cd calibration
c: \ calibration> python calibrate.py
{% endhighlight%}

On Linux, simply run:

{% highlight shell_session%}
~ $ cd Arduino / best-fit-calibration
~ / best-fit-calibration $ python2 calibrate.py
{% endhighlight%}
      
To complete the calibration, copy all the calibration parameters to the * variocal.cfg * file on the SD card

{%include manuelimg.md name="Calibrate_python.jpg"%}

{% highlight shell_session%}
Variocal.cfg file

[VERSION=1.0]

/* Calibration */
[VERTACCEL_GYRO_CAL_BIAS_00=0xff]
[VERTACCEL_GYRO_CAL_BIAS_01=0xff]
[VERTACCEL_GYRO_CAL_BIAS_02=0x3f]
[VERTACCEL_GYRO_CAL_BIAS_03=0xb3]
[VERTACCEL_GYRO_CAL_BIAS_04=0x00]
[VERTACCEL_GYRO_CAL_BIAS_05=0x00]
[VERTACCEL_GYRO_CAL_BIAS_06=0x00]
[VERTACCEL_GYRO_CAL_BIAS_07=0x00]
[VERTACCEL_GYRO_CAL_BIAS_08=0x01]
[VERTACCEL_GYRO_CAL_BIAS_09=0x00]
[VERTACCEL_GYRO_CAL_BIAS_10=0xf7]
[VERTACCEL_GYRO_CAL_BIAS_11=0xff]
[VERTACCEL_ACCEL_CAL_BIAS_00=4240]
[VERTACCEL_ACCEL_CAL_BIAS_01=12585]
[VERTACCEL_ACCEL_CAL_BIAS_02=17394]
[VERTACCEL_ACCEL_CAL_SCALE= -136]
[VERTACCEL_MAG_CAL_BIAS_00=11068]
[VERTACCEL_MAG_CAL_BIAS_01=20912]
[VERTACCEL_MAG_CAL_BIAS_02=17504]
[VERTACCEL_MAG_CAL_PROJ_SCALE=-17821]
[VERTACCEL_ACCEL_CAL_BIAS_MULTIPLIER=7]
[VERTACCEL_MAG_CAL_BIAS_MULTIPLIER=7]

{% endhighlight %}

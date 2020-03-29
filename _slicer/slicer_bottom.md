---
step: 2
title: 3Dcase
description: Bottom case
---

[Télécharger le profil]({{ 'assets/fichiers/profils3Dprinter/Geeetech_A20M_boitier_bas.fff' | relative_url }})

Once your file has been loaded into simplify3d, you will be able to change the profile settings to optimize printing.


{% include slicerimg.md name="Bottom_1.jpg" %}


**"Extruder" tab:** 


The distance and speed of retraction will depend on your printer. The vertical retraction elevator allows the nozzle to be lifted a little after a retraction and thus avoid touching the part during a movement.


{% include slicerimg.md name="Bottom 2.jpg" %}

**"Layer" tab**

For this part, 0.2mm layers are a good compromise between speed and print quality. With a first layer height of 150%, the first layer will be 0.3mm. A speed of 20% compared to the overall printing speed allows good grip, in particular screw and strap turns.


{% include slicerimg.md name="Bottom 3.jpg" %}

**"Additions" tab**

Adding a skirt around the case, just to purge the nozzle.



{% include slicerimg.md name="Bottom 4.jpg" %}

**"Infill" tab:**

Choice of 40% material and a honeycomb filling.


{% include slicerimg.md name="Bottom 5.jpg" %}

**"Support" tab**

Not necessary for this case. You can uncheck the box.

{% include slicerimg.md name="Bottom 6.jpg" %}

**"Temperature" tab**

Here you set the extrusion temperature of the PLA (Shared Heater, here 215 ° C) and the temperature of the heating plate (Heated Bed, here 60 ° C)

{% include slicerimg.md name="Bottom 7.jpg" %}

**"Cooling" tab**

With PLA, leave the default values: first layer without fan, next layer, fan at 100%.


{% include slicerimg.md name="Bottom 8.jpg" %}

**"G-Code" tab**

If you wish to use the downloadable profile at the top of the page, you can here modify the characteristics of your printer (Cartesian, delta, printing volume, etc.)


{% include slicerimg.md name="Bottom 9.jpg" %}

**"Scripts" tab**

Keep your printer's default scripts.


{% include slicerimg.md name="Bottom 10.jpg" %}

**"Speeds" tab**

The printing speed depends on the mechanical quality of your printer. At 60mm / s there should be no problems.

{% include slicerimg.md name="Bottom 11.jpg" %}

**"Other" tab**

Adjust the size of your filament, price, density ....


{% include slicerimg.md name="Bottom 12.jpg" %}

**"Advenced" tab**

Thin wall behavior: leave "Perimeter only" and "Allow filling of spaces".

{% include slicerimg.md name="Bottom 13.jpg" %}



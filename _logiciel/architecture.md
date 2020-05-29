---
step: 1
title: Firmware
description: Architecture
---

Here is the general description of the Gnuvario-E firmware

To operate the Gnuvario-E needs a firmware and an SD card with a particular organization

**Firmware**      
   
There are several firmware versions which correspond to the different screen versions and to beta or stable versions
   
-- For GNUVario-E with 1.54'' screen     --

Stable {% include lienfichier.md name="firmware" lien="update/Gnuvario154.bin" %}     
Beta {% include lienfichier.md name="firmware" lien="update/Gnuvario154b.bin" %} 

-- For GNUVario-E with 2.90'' screen in lanscape mode   --

Stable {% include lienfichier.md name="firmware" lien="update/Gnuvario290.bin" %}      
Beta {% include lienfichier.md name="firmware" lien="update/Gnuvario290b.bin" %} 

-- For GNUVario-E with 2.90'' screen in portrait mode-- 

Stable {% include lienfichier.md name="firmware" lien="update/Gnuvario291.bin" %}    
Beta {% include lienfichier.md name="firmware" lien="update/Gnuvario291b.bin" %}       

**SD Card**     

The SD card embeds a website and configuration files. There is a tree structure for the stable version and one for the beta version

RootSD for {% include lienfichier.md name="Stable firmware" lien="fichier/RootSD_Stable.zip" %}     
RootSD for {% include lienfichier.md name="Beta firmware" lien="fichier/RootSD_Beta.zip" %}    

**www folder**     

On the SD card, the www folder contains the files necessary for the operation of the embedded website. There is one version for the stable version and one for the beta version.

-- The versions for the 1.54 '' screen     --
   
www for {% include lienfichier.md name="Stable firmware" lien="dl-web/Gnuvario154" %}     
www for {% include lienfichier.md name="Beta firmware" lien="dl-web/Gnuvario154b" %}    

-- The versions for the 2.90 '' screen in landscape mode   --   
   
www for {% include lienfichier.md name="Stable firmware" lien="dl-web/Gnuvario290" %}     
www for {% include lienfichier.md name="Beta firmware" lien="dl-web/Gnuvario290b" %}    

--  The 2.90 '' screen versions in portrait mode   --    

www for {% include lienfichier.md name="Stable firmware" lien="dl-web/Gnuvario291" %}     
www for {% include lienfichier.md name="Beta firmware" lien="dl-web/Gnuvario291b" %}    

**AGL folder**

On the SD card, the ALG folder contains the files necessary for the AGL calculations (part of france, belgium, italia, swizerland and germany).
{% include logicielimg.md name="AGL.jpg" %}

[Download here the files for your region](https://vps.skybean.eu/agl/)

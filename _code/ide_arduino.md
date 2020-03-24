---
step: 1
description: Arduino IDE
---

To compile the GNUVario-E source code, you need the downloadable Arduino IDE [here](https://www.arduino.cc/en/Main/Software). Start by installing it and make sure you can launch the editor.

Next, you will add the management of ESP32 cards in the Arduino IDE

Go to the **"File"** then **"Preferences"** tab of the IDE and add the URL **https: //dl.espressif.com/dl/package_esp32_index.json** to the URLs of additional  board manager.

![GitHub zip download]({{"/assets/code_img/code11.jpg" | absolute_url}})

Then go to the tab **"Tools"**, **"card type"** and click on **"Card manager"**

![GitHub zip download]({{"/assets/code_img/code12.jpg" | absolute_url}})

Look for the **ESP32 by Espressif Systems** cards then click on install.

![GitHub zip download]({{"/assets/code_img/code13.jpg" | absolute_url}})


Now that the IDE is configured, you can retrieve the GNUVario-E source code.

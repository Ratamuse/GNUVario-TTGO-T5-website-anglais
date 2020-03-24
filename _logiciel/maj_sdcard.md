---
step: 4
title: Firmware
description: Update via SDcard
---

The Gnuvario firmware can be updated from the SD card.
Here is the procedure.

It is of course necessary to obtain this firmware beforehand; either from the Gnuvario website, or by compiling the sources yourself.

This file must be copied to the root of the SD card, with the name ** update.bin **; here is an example of the contents of the SD card after this copying, in wifi mode:

{% include logicielimg.md name="sdcardWithUpdate.bin.jpg"%}

At the next restart, the Gnuvario will detect the presence of this update.bin file, and will update from this code; the message 'upgrade in progress' will appear on the screen during the update process (about one minute).

{% include logicielimg.md name="upgradeBySDcard.jpg"%}

Then, the Gnuvario will restart automatically and start normal operation.

**Please note**: at the end of the update process, the file **update.bin** is automatically deleted.

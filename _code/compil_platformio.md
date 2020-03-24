---
step: 5
description: Compiling with VSCode - PlatformIO 
---

Beforehand, you must download the sources locally from the GIT repository.
The local directory must contain at least:
- the src / folder, which contains the Gnuvario-E.cpp file
- the lib / folder, which contains the necessary libraries
- the platformio.ini and custompart.csv files

{% include codeimg.md name="platformio_files.jpg"%}

In VSCode, click on the 'PlatformIO: Home' icon in the horizontal bar at the bottom. The PlatformIO Home page will appear in the IDE.

{% include codeimg.md name="platformio_home.jpg"%}

Click on 'Import Arduino Project'.
- select the 'board'. To speed up the selection, enter esp32, then choose 'Expressive ESP32 Dev Module'
- do not click 'Use libraries installed by Arduino IDE'
- select the folder that contains the code retrieved from the git repository
- click on the 'Import' button

{% include codeimg.md name="platformio_import_project.jpg"%}

The project appears in the left column (EXPLORER) of the IDE; it is possible to explore the different files of it.

{% include codeimg.md name="platformio_projet.jpg"%}

In the bottom horizontal bar, several icons linked to PlatformIO and the current project appear.
The most interesting icons are:
- (1). PlatformIO: Home: open the PlatformIO Home window
- (2). PlatformIO: Build: compile the code
- (3). PlatformIO: Upload: compile code, and load it into vario
- (8). Platformio: Serial Monitor: opening of a basic serial terminal

And now, if you want to compile the code and load it into the vario, you have to:
- start vario
- connect the vario to the PC via micro USB
- click on the PlatformIO: Upload icon

The compilation will be done. if no error, the compiled code will be loaded into the vario, and it will restart.

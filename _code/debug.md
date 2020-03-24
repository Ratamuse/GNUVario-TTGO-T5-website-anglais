---
step: 7
description: Debug
---

This chapter will describe the debugging methods used in the Gnuvario-E code.

Over time, the display system for debugging information has evolved.

Today there are 3 methods implemented in the Gnuvario-E code.

**Method 1**

Using the DebugConfig.h file and println
      
#define ENABLE_DEBUG
     
#define PROG_DEBUG // debug principal program
      
ENABLE_DEBUG allows to activate debugging.
     
Then for each type of information to be traced, we define or not define them.
The messages are displayed on the serial monitor by adding lines in the code.

#ifdef SCREEN_DEBUG
    SerialPort.print ("Created task: Executing on core");
    SerialPort.println (xPortGetCoreID ());
#endif // SCREEN_DEBUG


**Method 2**

Method 2 also uses the DebugConfig.h file but the poster is enriched with the name
source file, variable names and line.
     
At the start of each source file you must declare the use of debug functions.

#include <DebugConfig.h>
       
#ifdef NMEAPARSER_DEBUG
#define ARDUINOTRACE_ENABLE 1
#else
#define ARDUINOTRACE_ENABLE 0
#endif
     
#define ARDUINOTRACE_SERIAL SerialPort
#include <ArduinoTrace.h>

Then it will be possible to use the functions:

TRACE();
Displays line number, file name on serial monitor.
      
DUMP (someValue);
Display on the serial monitor the variable as well as the file and the line.
      
SDUMP (someText);
Display text, file and line on serial monitor.
       
**Method 3**
             
Method 3 records debugging information in the variolog.log file.
The debug.cfg file described in the "configuration" section is used to select messages to display.
          
You will have to use the variolog.h library.

The possible functions are:

TRACELOG (type, module)
Save the file and the line in the log file.

DUMPLOG (type, module, variable)
Save variable, file and line in log file.

MESSLOG (type, module, Text)
Record a message with the file and the line in the log file.

INFOLOG (Text)
Save a text in the log file.      
                                                                                                    


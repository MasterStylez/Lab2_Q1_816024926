# Lab2_Q1_816024926
P1

/project/sdkconfig is made using make menuconfig. This file is adjusted in my project
since i need a specific configuration for my ESP. Changing this file changes the 
flash settings.

/project/build/include/sdkconfig.h

This file is generated from the config file sdkconfig.

/sdk/components/freertos/port/esp8266/include/freertos/FreeRTOSConfig.h

This file initializes most freertos settings. It can be editted to change the default parameters,
or the changes can be made in a specific header file for the application.



P2

task.h is the header file we need to include
vTaskGetRunTimeStats is used to find task performance. It is included in task.h

The questions are split up into separate repositories. The links to the other repositories are below.

https://github.com/MasterStylez/Lab2_Q2a_816024926
https://github.com/MasterStylez/Lab2_Q2b_816024926
https://github.com/MasterStylez/Lab2_Q3_816024926

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
For task performance, configGENERATE_RUN_TIME_STATS, configUSE_STATS_FORMATTING_FUNCTIONS
and configSUPPORT_DYNAMIC_ALLOCATION must be set to 1.



Questions are split into branches, with one branch for questions 1, 2a, 2b and 3.




Question 2 Discussion.

I didn't expect the task priority to change much when using priority inheritence. This was observed.
my guess is that since the tasks can all run in a window without conflict, they would do so even
when the priorities shift.




Question 3 Discussion.

Sleeping affects system performance. With a small sleep, this change is likewise small. The time in which
the idle task was run increased.


---
title: Microcontroller 

## Overview
This project is for alerting device system that uses a speaker to warn you when something needs attention. It watches three different sensors: water,humidity, pressure problems. When any sensor detects a problem, the speaker sounds an alarm and a specific light turns on to tell you which kind of problem has found found.

# Testing
We started by just testing the lights and making sure they worked along the speaker. We made each light turn on one at a time for the given seconds in a repeating cycle. This proved the hardware was connected correctly.

# 
In the final code the system constantly checks all three sensors at the same time. The code now properly:
* Watches for water leaks and turns on a LED1 light with the speaker
* Watches for humidity problems and turns on a LED2 light with the speaker
* Watches for pressure issues and turns on a LED3 light with the speaker
* Alerts the speaker on as long as ANY sensor has a problem
* Turns everything off when all sensors are back to normal


## code test
![code test](projectpng/testcode.png).

## final code
![code](projectpng/code1.png).
![code](projectpng/code2.png).

## Example Microcontroller 

![Example of the Microcontroller ](projectpng/breadboard1.png).
![Example of the Microcontroller ](projectpng/breadboard2.png).
**Figure 1:** 

## Example Microcontroller Function
![Example Microcontroller Function ](projectpng/LED1.png)
![Example Microcontroller Function ](projectpng/LED2.png)
![Example Microcontroller Function ](projectpng/LED3.png)

**Figure 2:** 

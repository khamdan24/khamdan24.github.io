---
title: Hardware V2.0
---
## Overview
If we were to design a second version of this hardware, several improvements could be made to increase reliability, usability, and performance. These changes are based on lessons learned during prototyping and testing.

## Proposed Improvements

1. Revised PCB Layout
In V1, the PCB had measurement errors that prevented proper fitting into the enclosure. V2 would include:
* Accurate dimension checks before manufacturing
* Mounting holes aligned with the enclosure
* Better labeling of components for easier assembly

2. Improved Audio Output
The current speaker works for small rooms but may not be loud enough for noisy environments. V2 could:
* Use a higher-power amplifier (like TPA4411) for louder sound
* Include volume control via a potentiometer
* Add a small baffle or resonator in the enclosure to improve sound projection

3. Visual Alert Enhancements
* Use multi-color LEDs to show different alarm types (red for water, yellow for humidity, etc.)
* Add a flashing pattern for better visibility
* Include a small LCD or OLED screen to display sensor status messages

4. Connector Standardization
* Replace loose wire connections with standardized connectors (JST, header pins)
* This would make assembly faster and reduce wiring mistakes

These updates would make the system more reliable in real-world conditions, easier to install, and more effective at getting the user’s attention during an emergency.

---
title: Resource
---

# Code Testing
We started by just testing the lights and making sure they worked along the speaker. We made each light turn on one at a time for the given seconds in a repeating cycle. This proved the hardware was connected correctly.

# Final Code
In the final code the system constantly checks all three sensors at the same time. The code now properly:
* Watches for water leaks and turns on a LED1 light with the speaker
* Watches for humidity problems and turns on a LED2 light with the speaker
* Watches for pressure issues and turns on a LED3 light with the speaker
* Alerts the speaker on as long as ANY sensor has a problem
* Turns everything off when all sensors are back to normal


![Test Code](testcode.png).

**Figure 1:** 


![Code1](code1.png).
![Code2](code2.png).

**Figure 2:** 

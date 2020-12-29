# Cuckoo-Clock

Forked from R-Kearney

Got a Guzzini cuckoo clock with broken electronics.
Spare from China was more expensive then the whole clock.

Motor, speaker, trigger from clock and solenoid are directly connected to Arduino Nano and powered via 4x 1.2V battery pack.
LDO on Arduino is omitted and battery back is directly fed to VCC.

Changes to original version:

-Omit the LDR and use fixed times instead. Cuckoo just works between 8am and 7pm.
-Add power down mode to reduce power consumption (60mA without PD during idle, with PD 0.134mA!)
-trigger of clock movement is connected to wake up Arduino

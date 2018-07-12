Changes:
To prevent resin shield from blowing up these are the mods:
1. cut away the wire between the FAULT pin and the arduino.
2. double the number of catch diodes on the positive output to handle the short circuit current
3. add extra copper between +15 catch diode cathode and +15 output caps to reduce inductance
4. add 18V zener between FAULT pin and -15V to shut down the part in the case of excess voltage build up on unregulated channel
5. these problems are much easier solved with better layout and part selection
To make sure resin shield doesn't cycle on and off during startup:
1. remove all the EN/UVLO resistors
2. replace upper with 6.8k, bottom with 1k, series resistor to 0ohm


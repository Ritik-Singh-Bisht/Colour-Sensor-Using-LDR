# Colour-Sensor-Using-LDR
CONSTRUCTION
1) The Sensor consists of:- 
   -> 1 RGB LED 
   -> 1 LDR sensor
   -> 2  220 ohm resistors 
   -> 1 Arduino UNO
   -> 1 Breadboard, jumper wires.

2) LDR sensor is connected in series with a 220 ohm resistor and is connected to a 5V supply.   
3) Analog pin 5 reads the potential difference of the resistor connected to the sensor and converts it in a range from 0-1023.
4) One 220 ohm resistor is connected to the cathode of  the RGB LED.
5) The anodes of the red, green, blue LED are connected to the digital pin 13, 12, 11 of the arduino respectively. 

WORKING
1) When red light is incident on the LDR sensor, the reading of the sensor varies from 300-500.
2) When the sensor values are between this range, the arduino makes the digital pin 13 high and other pins low,i.e, RGB LED will glow red.
3) Similarly when analog pin reads between 100-165 and 165-300, arduino will make digital pin 12(green) and 11(blue) high respectively.
4) When no coloured light is incident on the LDR sensor, the sensor reads values lower than 100, then the arduino will make all the digital    pins of the RGB LED low and the LED will be in its off state.
5) The analog pin wil read value from the sensor at a interval of 2 seconds.

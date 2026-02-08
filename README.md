# Potentiometer (POT)

A potentiometer is a variable resistor which resistance can be controlled via rotating its knob. 

In this tutorial you will learn how to use a potentiometer with and without Arduino board to fade an LED.

[Potentiometer PINOUT](https://github.com/kingston-hackSpace/Potentiometer_LED/blob/main/PINOUT.png)

----
# Hardware

- Arduino UNO

- LED (x1)

- Potentiometer 10K

- Resistor 220ohms (x1)

----
# Wiring

Remember that LEDs have a positive and negative pin. You may burn the LED if wired incorrectly. See [here](https://github.com/kingston-hackSpace/Push-button_LED/blob/main/Understanding_LEDs.png)

Find how to wire the potentiometer in the tutorials below.

----
# Code and instructions

STEP 1: Printing POT values in the Serial Monitor 

Follow [this tutorial](https://www.build-electronic-circuits.com/arduino-potentiometer/)

How to open the Serial Monitor [here](https://github.com/kingston-hackSpace/Potentiometer_LED/blob/main/SerialMonitor.png)

STEP 2: Controlling the brightness of an LED with a POT

Follow [this tutorial](https://www.circuitgeeks.com/arduino-potentiometer-tutorial/)

----
# Understanding POT values

**READ**

To read values from the potentiometer, we connect it to any of the **analog pins** of our Arduino. Then, we use **analogRead();** to read the incoming values. 

Analog read will always provide values between **0 - 1023** 

**MAP**

Once we have these incoming values, we might need to **map** those values to make them useful values to activate another piece of equipment, such an LED.

**WRITE**

Our LED is connected to a PMW digital pin (~), which can modulate a signal in a range of values between 0 - 255 via analogWrite();

----
# Understanding the Map() function

The **map();** function "re-maps" a number from one range to another.

map(variable to be map, original min value, original max value, wanted min value, wanted max value);

For example:

```
int sensorValue = analogRead(A0); 
int brightness = map(sensorValue, 0, 1023, 0, 255); 
analogWrite(ledPin, brightness);
```

Read more [here](https://docs.arduino.cc/language-reference/en/functions/math/map/)

----
# MORE EXAMPLES

[LED Color Mixer](https://docs.arduino.cc/learn/electronics/potentiometer-basics/)

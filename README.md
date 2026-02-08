# Potentiometer (POT)

A potentiometer is a variable resistor that we can control via its knob. 

In this tutorial you will learn how to use a potentiometer with and without Arduino board to fade an LED.

----
# Setting up before starting

[Understanding Potentiometers]

[Potentiometer PINOUT](https://github.com/kingston-hackSpace/Potentiometer_LED/blob/main/PINOUT.png)

[Understanding LEDs](https://github.com/kingston-hackSpace/Push-button_LED/blob/main/Understanding_LEDs.png)

----
# Hardware

- Ardiuno UNO

- LED 

- Potentiometer 10K

- Resistor 220ohms

----
# Wiring

See diagram [here]

Remember that LEDs have a positive and negative pin. You may burn the LED if wired incorrectly. See [here](https://github.com/kingston-hackSpace/Push-button_LED/blob/main/Understanding_LEDs.png)

----
# Code and instructions

STEP 1: Printing values in the Serial Monitor 

Follow [this tutorial](https://www.build-electronic-circuits.com/arduino-potentiometer/)

How to open the Serial Monitor [here](https://github.com/kingston-hackSpace/Potentiometer_LED/blob/main/SerialMonitor.png)



----
# Understanding POT values

**READ**

To read values from the potentiometer, we connect it to any of the **analog pins** of our Arduino. Then, we use **analogRead();** to read the incoming values. 

Analog read will always provide values between **0 - 1023** 

**MAP**

Once we have does incoming values, we might need to **map** those values to make them useful values to activate another piece of equipment, such an LED.

**WRITE**

Our LED is connected to a PMW digital pin (~), which can module a signal in a range of values between 0 - 255 via digitalWrite();

----
# Understanding the Map() function

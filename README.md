# Potentiometer (POT)

A potentiometer is a variable resistor that we can control via its knob. 

In this tutorial you will learn how to use a potentiometer with and without Arduino board to fade an LED.

----
# Setting up before starting

[Understanding Potentiometers]

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

----
# Understanding POT values

As in the previous example, we connect potentiometers to any of the analog pins of our Arduino, and we use *analogRead();* to read the incoming values. 

Analog read will always provide values between **0 - 1023**.

Once we have does incoming values, we might need to *map*

----
# Map() function

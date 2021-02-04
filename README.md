# Finger-Print-Scanner
The Finger Print Scanner Library for Raspberry Pi

## Introduction

Not only in Hollywood films, fingerprint readers are seen more and more frequently. 
Such modules are often installed in home surveillance systems and are used for the simple but secure verification of persons. 
With such a Raspberry Pi Fingerprint Sensor you can also implement some other projects, such as secured locks.

One of the advantages is that passwords and / or number codes can be completely omitted. 
Although this is still possible, but it’s a lot more comfortable without. 
This tutorial is about the connection as well as the reading, saving and verifying of imported fingerprints.

## Accessories
These sensors were originally developed for the Arduino and can be read via UART.
The Raspberry Pi has two pins (pin 8 / GPIO14 and pin 10 / GPIO 15), but they work with 3.3V.
Since there are different fingerprint sensors, which do not all work with 3.3V, a USB UART converter is recommended.
Some models can be used with both 3.3V and 5V voltage. These are particularly suitable (also in connection with an Arduino).

The following is therefore required:
* Bullet listRaspberry Pi Fingerprint Sensor (US* / UK*). Apart from the voltage the models do not differ much.
*Bullet list[Serial USB converter (US* / UK*) with 3.3V and 5V connection]
*Bullet list[Female-Female Jumper wires (US* / UK*), if not included with the USB converter.]
*Bullet list[optional: cousing (which can also be 3d-printed)]


Note in the article description, what voltage your sensor needs.
Mine needs 3.3V input voltage, however, e.g. other models have a voltage between 3.8V and 6V.
The voltage is very important for the connection.

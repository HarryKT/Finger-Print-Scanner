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
* Raspberry Pi Fingerprint Sensor. Apart from the voltage the models do not differ much.
* Serial USB converter with 3.3V and 5V connection
* Female-Female Jumper wires, if not included with the USB converter.
* optional: cousing (which can also be 3d-printed)

Note in the article description, what voltage your sensor needs.
Mine needs 3.3V input voltage, however, e.g. other models have a voltage between 3.8V and 6V.
The voltage is very important for the connection.

## Installation of the Raspberry Pi Fingerprint Library
For some commands of the installation, root privileges are required.
Therefore we start a terminal session and type the following, which executes all the following commands as root:
````
sudo bash
````

Now we add the necessary package sources:
````
wget -O - http://apt.pm-codeworks.de/pm-codeworks.de.gpg | apt-key add -
wget http://apt.pm-codeworks.de/pm-codeworks.list -P /etc/apt/sources.list.d/
````

We then update the available packages and install the Python library:
````
apt-get update
apt-get install python-fingerprint --yes
````

If an error has occurred (in particular, that not all dependent packages have been installed), then execute the following:
````
apt-get -f install
````

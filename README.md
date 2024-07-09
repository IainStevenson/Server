# Server

A very simple Wew server sketch for an Arduino Mega 2560 board with an Ethernet shield

This is a slightly modified version of the Arduino Ethernet sample to learn how to use the PlatformIO plugin and environment works within VS Code

Lessons learned, 

On Linux

You need to get your Rules.d sorted as per the instructions in Platformio : https://docs.platformio.org/en/stable/core/installation/udev-rules.html

You need to ensure you are in the dialout group and the USB or whatever port you connect via is set correctly permissions wise.
You need to ensure that you can build and upload a very simple sketch before you do anything else jsut to make sure the Polatformio plugin is working correctly
Plugging the device in via a USB port hub (even when powered) did not work, Verification errors on upload occured.

Then in the Visual Studio code PlatformIO side bar

* Build
* Upload
* Monitor  (or just (Upload and Monitor)
* Then [in any browser call the device](http://192.168.0.177/) and you should see the data come back every 5 seconds.

leoTracker
==========

Small AVR-based standalone APRS Tracker for [Trackuino](http://www.trackuino.org/)

![leoTracker Front](/img/leoFront.jpg?raw=true)

This board was designed to be fairly inexpensive (BOM is $50 depending upon power source), small (1.25"x2.85"), light (under 20g depending upon configuration), and offer some features not yet available on other trackers.

Features include:

- On-board ublox MAX-7/8 GPS w/ chip antenna
- Multiple Power options including boost converter (2xAA operation)
- Atmel (AVR) 32u4 Processor (same as in the Arduino Leonardo - hence the "leo")
- On-board USB for easy firmware updates
- microSD socket for data logging/board configuration
- NiceRF SA818 2m radio module (frequency agile; multiple power levels)

Firmware
--------
The firmware is available at [github.com/kf7fer/trackuino](http://github.com/kf7fer/trackuino). It is modified from the [John Boiles Port](https://johnboiles/trackuino/) in order to support the different pin mappings used on the leoTracker (as well as support of additional hardware).

Changes to the firmware include:

- Support for the ublox MAX-6/7/8 (switch to flight mode; use low power mode when possible)
- Support for the on-board microSD card (still a work in progress)
- Support for the Dallas DS18b20 temperature sensors (two are supported)
- Added support for the NiceRF SA818 radio module


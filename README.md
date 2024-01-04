# Adafruit MMC56x3 Magnetometer Library
## Archive note
This is now archived because I have replaced it in the project I needed it for. And I only created this because of a very obscure issue I had.

## Modifications ##
Replaced `sensor_t` with `adafruit_sensor_t`, reasons listed in README [here](https://github.com/chopster44/Adafruit_Sensor). Also modified the README a bit.

***

This library is for the Adafruit MMC5603 or MMC5613 Breakouts

Tested and works great with Adafruit's MMC5603 Breakout Boards
* https://www.adafruit.com/product/5579

This chip uses I2C to communicate, 2 pins are required to interface

Adafruit invests time and resources providing this open source code, please support Adafruit and open-source hardware by purchasing products from Adafruit!

## About the MMC5603 ##

The MMC5603 is a 3-axis magnetometer made by Memsic. The magnetometer measures magnetic force, which is useful to detect magnetic north.

More information on the MMC5603 can be found in the datasheet: https://media.digikey.com/pdf/Data%20Sheets/MEMSIC%20PDFs/MMC5603NJ_RevB_7-12-18.pdf


## What is the Adafruit Unified Sensor Library? ##

The Adafruit Unified Sensor Library (**Adafruit_Sensor**) provides a common interface and data type for any supported sensor.  It defines some basic information about the sensor (sensor limits, etc.), and returns standard SI units of a specific type and scale for each supported sensor type.

It provides a simple abstraction layer between your application and the actual sensor HW, allowing you to drop in any comparable sensor with only one or two lines of code to change in your project (essentially the constructor since the functions to read sensor data and get information about the sensor are defined in the base Adafruit_Sensor class).

This is imporant useful for two reasons:

1.) You can use the data right away because it's already converted to SI units that you understand and can compare, rather than meaningless values like 0..1023.

2.) Because SI units are standardised in the sensor library, you can also do quick sanity checks working with new sensors, or drop in any comparable sensor if you need better sensitivity or if a lower cost unit becomes available, etc. 

Light sensors will always report units in lux, gyroscopes will always report units in rad/s, etc. ... freeing you up to focus on the data, rather than digging through the datasheet to understand what the sensor's raw numbers really mean.

## About this Driver ##

Written by ladyada for Adafruit Industries.
Modified by Chopster44.
BSD license, check license.txt for more information
All text above must be included in any redistribution

To install, use the Arduino Library Manager and search for "Adafruit MMC56x3" and install the library.

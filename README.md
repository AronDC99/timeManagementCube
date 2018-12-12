# Time management cube

## Hardware ideas

Control board - [Arduino Micro]( https://store.arduino.cc/arduino-micro)

Gyroscope - [MPU-6050](https://www.sparkfun.com/products/11028)

Bluetooth - [Bluefruit LE UART(BLE)](https://www.adafruit.com/product/2479)

## Project idea

 We intend to create a simple cube that contains 3 things, an arduino micro, a bluetooth module, a gyroscope and an accelerometer. This cube will then send the data it registers from the acc and gyro through the bluetooth module to an android device. The android device will then automatically translate the data from the cube into a schedule based on what side the cube is sittig on and export it into a readable format possibilities include: Google Calendar, exel doc, internal calculations in the app to display time spent in easy to view formats like pie charts and graphs.


## Wiring diagram
![wiring diagram](https://cdn.instructables.com/F8H/MG4X/IIYWU9A6/F8HMG4XIIYWU9A6.LARGE.jpg?auto=webp&width=836)


## Code setup
The first step is to download [this zip library](https://github.com/jrowberg/i2cdevlib/zipball/master) and extract I2Cdev and MPU6050 libraries to the arduino compilers library folder located in "C:/Program Files(x86)/Arduino/libraries".

Then it is possible to upload and compile the code on an arduino board of your choice we reccomend the arduino micro because of its size, if you have followed the wiring schematic above correctly you should be able to read the raw accelorometer and gyroscope data in the serial monitor straight from the arduino IDE.

# Time management cube

## Hardware ideas

Control board - [Arduino Micro]( https://store.arduino.cc/arduino-micro)

Gyroscope - [6 axis gyro and Acc](http://wiki.seeedstudio.com/Grove-6-Axis_AccelerometerAndGyroscope/)

Bluetooth - [Bluefruit LE UART(BLE)](https://www.adafruit.com/product/2479)

## Project idea

 We intend to create a simple cube that contains 3 things, an arduino micro, a bluetooth module, a gyroscope and an accelerometer. This cube will then send the data it registers from the acc and gyro through the bluetooth module to an android device. The android device will then automatically translate the data from the cube into a schedule based on what side the cube is sittig on and export it into a readable format possibilities include: Google Calendar, exel doc, internal calculations in the app to display time spent in easy to view formats like pie charts and graphs.

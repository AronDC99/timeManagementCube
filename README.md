# Time management cube

## Hardware

Control board - [Arduino Micro]( https://store.arduino.cc/arduino-micro)

Gyroscope - [MPU-6050](https://www.sparkfun.com/products/11028)

Bluetooth - [Bluefruit LE UART(BLE)](https://www.adafruit.com/product/2479)

## Project idea

 We intend to create a simple cube that contains 3 things, an arduino micro, a bluetooth module, a gyroscope and an accelerometer. This cube will then send the data it registers from the acc and gyro through the bluetooth module to an android device. The android device will then automatically translate the data from the cube into a schedule based on what side the cube is sittig on and export it into a readable format possibilities include: Google Calendar, exel doc, internal calculations in the app to display time spent in easy to view formats like pie charts and graphs.


## Gyroscope wiring diagram
![wiring diagram](https://cdn.instructables.com/F8H/MG4X/IIYWU9A6/F8HMG4XIIYWU9A6.LARGE.jpg?auto=webp&width=836)


## Code setup
The first step is to download [this zip library](https://github.com/jrowberg/i2cdevlib/zipball/master) and extract I2Cdev and MPU6050 libraries to the arduino compilers library folder located in "C:/Program Files(x86)/Arduino/libraries".

Then it is possible to upload and compile the code on an arduino board of your choice we reccomend the arduino micro because of its size, if you have followed the wiring schematic above correctly you should be able to read the raw accelorometer and gyroscope data in the serial monitor straight from the arduino IDE.

## BLE(Bluetooth Low Energy) module wiring diagram
![BLE wiring diagram](https://cdn-learn.adafruit.com/assets/assets/000/025/182/large1024/adafruit_products_UARTFriend_bb.png?1430515112)

## Android app setup
The android app should be installed with the .apk file on the client phone with android api 25 or higher

The app will prompt you for a connection to a bluetooth device and data will start transmitting automatically upon pairing the devices together.

### Other
Wiring diagrams are shown for the arduino Uno board, the same pins are available on the arduino micro other boards have not been tested by us and therefore some adaptation of hardware or software may be required


# Result

In the end we were unfortunately not able to complete this project for a multitude of reasons, despite the project not having been tested with the accelorometer and gyroscope every aspect of the project has been completed to an approved aspect, In theory with a functioning supported accelorometer and gyroscope the project should transmit the raw accelorometer and gyroscope data to the android app.


## "Broken" gyroscope
We had trouble with this [6 axis accelorometer and gyroscope](http://wiki.seeedstudio.com/Grove-6-Axis_AccelerometerAndGyroscope/) despite our best efforts we were unable to get a reliable reading from the module with only an arduino. If we were to use this specific module we would need to have an I2C translator board for the arduino to be able to read the data we also tested a vex robotics gyroscope but that gyroscope had the same problem with the required I2C board.

### Authors
[Yngvi Leó Þráinsson](https://github.com/DonNinja)
[Aron Davíð Clausen](https://github.com/arondc99)

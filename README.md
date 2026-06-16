# HRModel1
First Model Rocket with a flight computer to track barometric pressure, altitude, stability, acceleration, temperature, and direction relative to Earth's magnetic fields.

## Features
*Track data about your rocket's flight to analyze after the flight.

*Run IMU data into a Python script to display rocket stability throughout the whole flight.

*See changes in pressure and temperature as altitude increases.

*Hertz adjustable by changing variables IMURPS and BMPRPS (1-1000).

--> Both variables can be adjusted when the function is declared. 

--> Be careful with how many readings per second you can take, given your microcontroller's strength.

## Hardware
*Arduino Uno/Nano: Main "Brain" for the computer.
--> Can substitute with ESP32 but change SCL and SDA pins to GPIOs 22 and 21, respectively.
*BMP280: Logging barometric pressure, temperature, and altitude.
*IMU 9 Axis (MCU-20948 ICM-20948): Logs data on magnetic fields, has a gyroscope, and an accelerometer.
*Silicon Power 16GB Micro SD-Card: Stores data

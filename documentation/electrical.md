# Electrical

## Summary of Boards

### Brain Board
MCU
- V0 Board is a Teensy 4.0 Carrier Board
    - V1 Board will use a MCU from the same series. V0 decision made to speed development.
- Neopixel integrated
- SPI Flash memory
- Micro SD
- Physical arm switch

### GPS
U-blox ZED-F9R

### IMU
- Board with sensors and sensor fusion processing

| Sensor | Manufacturer | Model |
| - | - | - |
| IMU | Bosch | BMI088 |
| High-G Accelerometer | Analog Devices | ADXL375BCCZ |
| Low-G Accelerometer | Analog Devices | ADXL345 |
| Gyroscope | ST | A3G4250D |
| Barometer | TE | MS561101 |
| Magnetometer | PNI | RM3100 |

### IO Board
Inputs and outputs, as well as pyro switches

### Radio Board
Radio communication with ground control
- RFD900X Module

### Power Management Board
Creates voltages off battery to distribute to system
- 3.3V@<F3>3A 5V@3A V<sub>batt</sub>
- 6.5V - 16V XT30 input

## Standards

### Interconnect
HiRose DF17 30 pin

### Interconnect mapping

| # | Assingment | Assingment | # |
| - | ---------- | ---------- | - |
| 0 | V<sub>batt</batt> | 3.3V | 29 |
| 1 | V<sub>batt</batt> | 3.3V | 28 |
| 2 | GND | 5V | 27 |
| 3 | GND | 5V | 26 |
| 4 | RADIO TX | NEOPIXEL | 25 |
| 5 | RADIO RX | AUDIO | 24 |
| 6 | Unused | CAN1 HI | 23 |
| 7 | Unused | CAN1 LO | 22 |
| 8 | GPS RX | GND | 21 |
| 9 | GPS TX | GND | 20 |
| 10 | 5V | CAN2 HI | 19 |
| 11 | 3.3V | CAN2 LO | 18 |
| 12 | 1PPS | 3.3V | 17 |
| 13 | GND | Unused | 16 |
| 14 | GND | Unused | 15 |

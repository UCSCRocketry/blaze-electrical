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
| 4 | RADIO TX | Unused | 25 |
| 5 | RADIO RX | Unused | 24 |
| 6 | Unused | CAN HI | 23 |
| 7 | Arm | CAN LO | 22 |
| 8 | Unused | GND | 21 |
| 9 | Unused | GND | 20 |
| 10 | 5V | Unused | 19 |
| 11 | 3.3V | Unused | 18 |
| 12 | GPS PPS | 3.3V | 17 |
| 13 | GND | Unused | 16 |
| 14 | GND | Unused | 15 |

## Common Co-Processor and CAN Transceiver
A common design for a co-processor and CAN transceiver was developed in order to improve design flow and system performance.
The co-processor selected is the STM32H503KBUx, it features an ARM Cortex M33 clocked at 250MHz, 128KB of onboard flash memory, and 32 Kb of RAM.
The CAN tranciever selected is the TCAN1044VDDFR offering up to 8Mbps of full duplex CAN-FD communication 



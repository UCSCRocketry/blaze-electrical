# Electrical
## Summary of Boards
GPS
- GPS Module with antenna that can interface with Picofusion sensor fusion
- TODO: Spec antenna

IMU
- Board with sensors and sensor fusion processing

| Sensor | Manufacturer | Model |
| - | - | - |
| IMU | Bosch | BMI088 |
| High-G Accelerometer | Analog Devices | ADXL375BCCZ |
| Low-G Accelerometer | Analog Devices | ADXL345 |
| Gyroscope | ST | A3G4250D |
| Barometer | TE | MS561101 |
| Magnetometer | PNI | RM3100 |

Brain Board
- MCU
- V0 Board is a Teensy 4.0 Carrier Board
    - V1 Board will use a MCU from the same series. V0 decision made to speed development.
- Interconnect to IO board
- Neopixel integrated and output
- SPI Flash memory - Winbond W25
- Micro SD
- AUX power in
- Physical arm switch

IO Board
- Inputs and outputs, as well as pyro switches
- TODO: List input and output requirements

Radio Board
- Radio communication with ground control
- TODO: Compare radio options

Power Management Board
- Creates voltages of battery for rest of boards
- 3.3V 5V V<sub>batt</sub>
- 2S (7.4V) - 3S (11.1V) LiPo XT60 input
- TODO: Determine current requirement

## Standards
Footprint
- 45mm round

Interconnects
- HiRose DF17 30 pin
- Interconnect map

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

## Development Order
1. Brain Board v0
2. Power Management Board
3. IO Board
4. Radio Board
5. GPS Board

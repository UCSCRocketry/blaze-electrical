# Electrical
## Summary of Boards
GPS
- GPS Module with antenna that can interface with Picofusion sensor fusion
- TODO: Spec antenna

Picofusion
- External blob with sensors and sensor fusion
- TODO: Communicate interconnect

Brain Board
- MCU
- TODO: OS Processing power requirements

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
- 50mm round

Interconnects
- HiRose DF17U
- TODO: Determine pinout and # positions and location
- Belongs on interconnect:
-- 5V
-- 5V
-- 3.3V
-- 3.3V
-- 3.3V
-- 3.3V
-- V<sub>batt</sub>
-- V<sub>batt</sub>
-- GND
-- GND
-- GND
-- GND
-- GND
-- CAN1 Hi
-- CAN1 Lo
-- CAN2 Hi
-- CAN2 Lo
-- UART Rx
-- UART Tx
-- 1PPS


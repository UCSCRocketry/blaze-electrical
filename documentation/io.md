# Input Output (IO)
The Blaze IO board provides external inputs and outputs to the system. Four channels of MOSFETS allow pyro charges to be triggered on battery voltage. These outputs are protected by a physical arm switch. Outputs for 5V servos can be used to control TVC, active fins, and other control systems.
     
Blaze IO utilizes the common Blaze co-processor and transceiver described in the common documentation.

## STM32 STM32H503KBUx Pin Mapping

| Port | Physical Pin | Use | Function |
|-----|-----------|------|----------|
|PB5|28|CAN RX|Input|
|PB6|29|CAN TX|Output|
|PA0|6|Fet A|Output|
|PA1|7|Fet B|Output|
|PA2|8|Fet C|Output|
|PA3|9|Fet D|Output|
|PA4|6|Fet A Sense|Input|
|PA5|7|Fet B Sense|Input|
|PA6|8|Fet C Sense|Input|
|PA7|9|Fet D Sense|Input|

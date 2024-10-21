# Blaze Brain v0
Blaze Brain is the name given to the main processing board. This board is responsible for in taking information from all other boards, performing data logging, guidance and control calculations, and other tasks as well as outputting data to output boards.

The initial version of this board uses a Teensy 4.0 mounted to the board to accelerate software developments. Future versions will have the MCU directly on the board, and then will eventually have am upgraded MCU.

## Component Selection

| Ref | Component | Mfg. | Mfg. Part|Note|
|-----|-----------|------|----------|----|
|1|MCU|PJRC|TEENSY40||
|2|NeoPixel|AdaFruit|WS2812B|DI Physical Pin 6|
|3|Flash|WinBond|W25N02KVZEIR|Hardware CS Physical Pin 10|
|4|MicroSD|Molex|472192001|Bit Bang CS Physical Pin 9|
|5|SD FET|ON|FDN340P|Inrush current limiting for SD|

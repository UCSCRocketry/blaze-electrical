# Power Management
The power management system is designed to provide reliable, redundant, clean power to the entire Blaze system. The power is generated using multiple buck converters powered by a battery with a hard power switch. Dedicated current and voltage sensing allows for precise current and voltage spike event detection as well as battery charge monitoring. Reverse current and resettable over current protection enables for safe operation with minimal downtime. LED indicators visibly show voltage rails present.

Battery and hard power switch are connected through XT30 connectors.

Blaze PowerMan utilizes the common Blaze co-processor and CAN transceiver design described in the common documentation.

## Specs

|Spec|Value|
|-|-|
|VIN Max|16V|
|VIN Min|6.5V|
|Current Draw Max|6A|
|3V3 Current|3A|
|5V Current|3A|

## Component Selection

| Ref | Component | Mfg. | Mfg. Part|Note|
|-----|-----------|------|----------|----|
|1|Buck Controller|TI|TPS62913||
|3|Rev. Current PMOS|Diodes|DMG2305UX||
|4|Polyfuse|?|?||
|5|Current Sense Amplifier|TI|INA2181||

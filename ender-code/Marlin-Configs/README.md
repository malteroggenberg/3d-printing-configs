\# Marlin Firmware Configuration – Ender 3 (SKR Mini E3 V1.2)



\## Overview



This repository contains a custom configuration for Marlin Firmware, specifically tailored for a modified Ender 3 setup.



The firmware was originally created as a \*\*fallback solution in case of Raspberry Pi / Klipper failure\*\*, allowing the printer to run standalone.



\## Hardware Setup



\* Printer: Ender 3

\* Mainboard: BTT SKR Mini E3 V1.2

\* Extruder: Sprite Extruder

\* Bed Leveling: BLTouch (clone)

\* Filament Runout Sensor: Connected to PC14



\## Key Features / Modifications



\* Configuration optimized for Sprite Extruder

\* BLTouch integration with \*\*shortened probing sequence\*\*

\* Custom runout sensor pin assignment (PC14)

\* Stable standalone operation without external host (e.g. Raspberry Pi)



\## Files Included



\* `Configuration.h`

\* `Configuration\_adv.h`



These files are intended to be used with the official Marlin Firmware source.



\## Usage



1\. Download the official Marlin Firmware:

&#x20;  https://github.com/MarlinFirmware/Marlin



2\. Replace the configuration files with the ones from this repository.



3\. Build the firmware using PlatformIO, for example:



&#x20;  ```

&#x20;  pio run -e STM32F103RC\_btt\_USB

&#x20;  ```



4\. Flash the firmware by copying the generated `firmware.bin` file to an SD card and inserting it into the printer.



\## Notes



\* This configuration is highly hardware-specific.

\* Especially the BLTouch setup and probe behavior are tuned for this exact setup.

\* The shortened probing sequence may not work correctly on other machines.



\## License / Disclaimer



This configuration is intended for use with Marlin Firmware (GPLv3).



No Marlin source code is included in this repository.

All rights to the original firmware belong to the Marlin developers.



For the full source code and license details, please refer to the official repository:

https://github.com/MarlinFirmware/Marlin



This repository only provides configuration files.

Use at your own risk.


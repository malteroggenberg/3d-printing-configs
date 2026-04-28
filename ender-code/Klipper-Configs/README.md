\# Klipper Configuration – Ender 3 (Custom Setup)



\## Overview



This repository contains a customized Klipper configuration for an \*\*Ender 3\*\*.



The configuration was originally based on an Ender 2 setup but has been \*\*adapted, tested, and calibrated for the Ender 3\*\*.



The focus of this setup is improved performance, higher print speeds, and reliable probing using BLTouch.



\## Key Modifications



\* Migrated from Ender 2 configuration → fully adapted to Ender 3

\* Calibrated and tested on Ender 3 hardware

\* Increased printing speeds

\* Updated PID tuning (hotend / bed)

\* Retraction set to \*\*1.5 mm\*\*

\* Stepper configuration verified and stable



\## BLTouch Setup



\* BLTouch connected to \*\*Z-Endstop pin\*\*

\* Probing configured to cover \*\*maximum reachable bed area\*\*

\* Optimized probing behavior for efficient bed leveling



⚠️ Important:



\* \*\*Z-offset must be calibrated individually\*\*

\* \*\*Home position (X/Y) may need adjustment depending on your printer\*\*



\## Extruder Configuration



\* Currently configured for:



&#x20; \* \*\*BMG Extruder (3:1 gear ratio)\*\*



⚠️ Not yet adapted for Sprite Extruder

→ Extruder parameters (e.g. rotation distance) must be adjusted if changed



\## Additional Notes



\* Virtual SD Card is configured for \*\*OctoPrint\*\*



&#x20; \* Path must be adjusted depending on your setup



Example:



```

\[virtual\_sdcard]

path: \~/printer\_data/gcodes

```



\* Always verify hardware-specific parameters before use



\## Files



\* `printer.cfg`

\* Additional config / macro files (if included)



\## Setup / Usage



1\. Install Klipper on your host system (e.g. Raspberry Pi)

2\. Copy the configuration files to:



&#x20;  ```

&#x20;  \~/printer\_data/config/

&#x20;  ```

3\. Adjust:



&#x20;  \* Z-offset

&#x20;  \* Probe area / bed size

&#x20;  \* Extruder configuration

&#x20;  \* Virtual SD path

4\. Restart Klipper:



&#x20;  ```

&#x20;  sudo service klipper restart

&#x20;  ```



\## License / Disclaimer



This configuration is intended for use with Klipper Firmware (GPLv3).



No Klipper source code is included in this repository.

All rights to the original firmware belong to the Klipper developers.



For the full source code and documentation, refer to the official repository:

https://github.com/Klipper3d/klipper



This repository only provides configuration files.

Use at your own risk.




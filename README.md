# 3D Printing Configs & Profiles

A structured collection of my personal 3D printing configurations, including **Bambu Studio profiles, Klipper setups, and Marlin firmware configurations**.

This repository documents real-world tuned settings across different printers, hardware modifications, and firmware approaches — ranging from legacy setups to current workflows.

## Contents

* **Bambu Studio**
  Tuned filament and process profiles for everyday use and optimized print quality.

* **Klipper Configurations**
  Performance-oriented configs with calibrated motion systems, BLTouch setups, and higher-speed tuning.

* **Marlin Configurations**
  Legacy firmware setups used as fallback solutions and for standalone printer operation.

## Purpose

* Keep a **versioned backup** of all configurations
* Provide **reproducible setups** for different hardware configurations
* Document the evolution from **Marlin → Klipper → Bambu ecosystem**

## Notes

* All configurations are **hardware-specific** and may require adjustments
* Especially important parameters:

  * Offsets (Z, probe)
  * Bed size / probe area
  * Extruder configuration
* Use as a **reference or starting point**, not as plug-and-play configs

## Repository Structure

Each folder contains its own README with detailed explanations and usage instructions.

## Disclaimer

This repository only contains configuration files.
No firmware source code is distributed.

Use at your own risk.

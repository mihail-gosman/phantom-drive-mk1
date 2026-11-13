# Phantom Drive Mk I

> Open-source, 3D-printed 6-DOF industrial robotic manipulator engineered for repeatable precision, modular GT2 belt drives, and real-time motion control.

![Status](https://img.shields.io/badge/Status-In_Development-orange)
![Hardware License](https://img.shields.io/badge/Hardware_License-CERN--OHL--P_v2-blue)
![Software License](https://img.shields.io/badge/Software_License-Apache_2.0-green)
![CAD](https://img.shields.io/badge/CAD-FreeCAD-red)

## System Specifications

| Parameter | Specification |
| :--- | :--- |
| **Architecture** | 6-DOF Articulated Robotic Arm |
| **Primary Structure** | 3D-Printed Composite (`PETG-CF` / `PA12-CF`) + COTS Hardware |
| **Transmission** | GT2 Timing Belt Reduction (`J1`–`J6`) |
| **Electronics** | Modular Stepper Drivers + Microcontroller + Hardware E-Stop |
| **Firmware & Control** | Real-Time C++ (`PlatformIO`) + Python / ROS 2 Kinematics |

## Repository Structure

* **`bom/`** — Master Bill of Materials (`master_bom.csv`) covering printed, machined, and COTS components.
* **`mcad/`** — Mechanical CAD: purchased hardware (`cots/`), native FreeCAD parametric models (`source/`), neutral exports (`step/`), ready-to-slice meshes (`additive/`), and 2D drawings (`fab/`).
* **`ecad/`** — Electrical CAD: system-level module schematics (`schematics/`) and WireViz cable/pinout documentation (`harness/`).
* **`firmware/`** — Real-time deterministic microcontroller code (`PlatformIO`).
* **`software/`** — High-level kinematics, host control scripts, and URDF simulation models.
* **`docs/`** — Assembly work instructions, electrical safety procedures, calibration guides, and media.

## Acknowledgments

Inspired by open and prosumer 6-DOF desktop robotic arms such as Arctos. **Phantom Drive Mk I** is an independent, ground-up design with original CAD, schematics, and code, and is not affiliated with or endorsed by any third-party brand.

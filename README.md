# GAEL'S RP2040 Board

![Top View](https://raw.githubusercontent.com/yourusername/rp2040-board/main/images/3D_viewer_top_side.jpg)
![Bottom View](https://raw.githubusercontent.com/yourusername/rp2040-board/main/images/3D_viewer_bottom_side.jpg)

## Overview

This repository contains the complete KiCad project, schematic, PCB layout, 3D renders, and images of the final assembled board for **Gael’s custom RP2040 development board**. It includes a USB-C power interface, LIS3DH accelerometer for motion sensing, push buttons, LEDs, and header pins for debugging and expansion. 

Designed to be compact and circular, this board is suitable for embedded applications, including wearable tech and motion-aware devices.

---

## Features

- **Microcontroller:** Raspberry Pi RP2040
- **Accelerometer:** STMicroelectronics LIS3DH (3-axis, I2C)
- **Debug Header:** SWDIO, SWCLK
- **Buttons:** 3 tactile push buttons
- **LEDs:** 4 indicators
- **USB:** USB Micro-B for power and programming
- **Power Supply:** 3.3V regulated via AMS1117
- **Clock:** 12 MHz crystal oscillator
- **Form Factor:** Custom round PCB

---

## Hardware Components

| Component       | Description                                                       | Datasheet / Link |
|----------------|-------------------------------------------------------------------|------------------|
| [RP2040](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html) | Dual-core ARM Cortex M0+ microcontroller | [PDF Datasheet](https://datasheets.raspberrypi.com/rp2040/rp2040-datasheet.pdf) |
| [LIS3DH](https://www.st.com/en/mems-and-sensors/lis3dh.html)                     | Low-power 3-axis accelerometer             | [PDF Datasheet](https://www.st.com/resource/en/datasheet/lis3dh.pdf) |
| [AMS1117-3.3](https://www.advanced-monolithic.com/pdf/ds1117.pdf)                | 3.3V Linear Voltage Regulator              | [PDF Datasheet](https://www.advanced-monolithic.com/pdf/ds1117.pdf) |
| USB Micro-B Connector | USB interface for power and programming           | [Example Part](https://www.sparkfun.com/products/9966) |
| 12 MHz Crystal Oscillator | Provides clock source for RP2040                    | [Typical Part](https://www.digikey.com/en/products/detail/ecs-inc/ECS-120-12-33A-EN/3083686) |

---

## Project Structure

```bash
📁 rp2040-board/
├── hardware/
│   ├── RP2040.kicad_sch        # KiCad schematic
│   ├── RP2040.kicad_pcb        # KiCad PCB layout
│   ├── gerbers/                # Gerber fabrication files
├── images/
│   ├── 3D_viewer_top_side.jpg
│   ├── 3D_viewer_bottom_side.jpg
│   ├── Front_and_Back_Layout.jpg
│   ├── Fully_soldered.jpg
│   ├── Fully_soldered_back.jpg
├── README.md                   # Project documentation

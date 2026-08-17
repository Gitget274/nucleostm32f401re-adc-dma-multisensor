# STM32F401RE Multi-Sensor ADC Acquisition & Time Averaging

A C firmware project developed in **STM32CubeIDE** for the **NUCLEO-F401RE** development board.

This program performs continuous analog-to-digital conversions (ADC) from three external sensors (a potentiometer, a temperature sensor and a light sensor) using **DMA (Direct Memory Access)** for efficient hardware-driven data transfers without CPU overhead. It computes a time average for each sensor measurement and continuously outputs the formatted real-time readings via UART.

---

## Table of Contents
- [Hardware & Electronic Components](#hardware--electronic-components)
- [How to Run](#how-to-run)
- [License](#license)

---

## Hardware & Electronic Components

Below is the list of electronic hardware and components required to build and test this project:

| Component | Quantity | Description / Notes |
| :--- | :---: | :--- |
| **STM32 Nucleo-F401RE** | 1 | Development board|
| **Potentiometer** | 1 | 10kΩ Bourns 91A1A-B28_B15L |
| **Light Sensor** | 1 | TEPT4400 |
| **Temp Sensor** | 1 | LM60BIZ/NOPB |
| **Passive Components** | As needed | Resistors and capacitors for sensor biasing/filtering (refer to datasheets for exact values) |
| **Breadboard & Wires** | 1 | Standard breadboard and DuPont jumper wires (M-M, M-F) |
| **USB Cable** | 1 | Mini-USB cable for programming, debugging, and serial monitoring |

---

## How to Run

1. Download the source code as a ZIP archive.
2. Extract the contents of the ZIP file into a folder named `nucleostm32f401re-adc-dma-multisensor`.
3. Open **STMicroelectronics STM32CubeIDE**.
4. Go to `File` > `Open Projects from File System...` and select the extracted folder to import and launch the project.

---

## License

This project is licensed under the **MIT License** - see the LICENSE file for details.

### Third-Party & Driver Licenses
The `Drivers/` directory contains libraries provided by STMicroelectronics and ARM:
- **STMicroelectronics HAL Drivers**: Licensed under the **BSD 3-Clause License**.
- **CMSIS & Core Components**: Licensed under the **Apache License, Version 2.0**.

All original copyright, patent, trademark, and attribution notices remain preserved as required by their respective licenses.

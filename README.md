# ESP32-S3-DevBoard-v1.0

## Overview
This project is the first version of my **ESP32-S3**. The purpose of this board is to act as a **wireless communication, expansion, and development support board**.

This board is intended to handle **higher-level support functions** such as wireless communication, sensor interfacing, debugging, and future peripheral expansion.

This is **Version 1.0**, meaning the primary goal was to design and lay out a functional first revision that establishes the core architecture for future integration and testing.

---

## Project Goals
The main goals of this board were to:

- Build a **modular companion board** for a future platforms
- Create a hardware platform around the **ESP32-S3**
- Add support for **wireless communication and external peripherals**
- Provide **easy bring-up, programming, and debugging access**
- Establish a foundation for future onboard communication, telemetry, and sensor expansion

---

## Current Features

### Core Hardware
- **ESP32-S3 WiFi module**
- **4-layer PCB design**
- **USB-C power input**
- **LM1117DT-3.3V LDO regulator**
- **ESP-PROG compatible programming/debug header**

### User / Bring-Up Features
- **BOOT switch**
- **RESET switch**
- **USER switch**
- **RGB LEDs**
- **Green power LED**

### Sensor / Expansion Features
- **SI7021-GMR temperature and humidity sensor** on the **I2C bus**
- **QWIIC connector** for external I2C peripherals
- **2x5 SPI expansion header**
  - planned for future peripherals such as a **W5500 Ethernet module**

### Mechanical
- **3.2 mm mounting holes**

---

## PCB Stack-Up
This board was designed as a **4-layer PCB** to improve routing flexibility, grounding, and power distribution.

### Stack-Up
- **Top Layer**
- **0.196 mm prepreg**
- **Inner Layer 1**
- **1.03 mm core**
- **Inner Layer 2**
- **0.196 mm prepreg**
- **Bottom Layer**

This stack-up was chosen to provide a better structure for embedded routing compared to a simpler 2-layer design.

---

## Why I Built This
I wanted to start building the electronics architecture for my own **autonomous drone system** rather than only working with off-the-shelf development boards.

This board is one of the first major hardware building blocks in that process.

The idea is to split the system into multiple roles:

- **STM32 board** → real-time flight control / lower-level control tasks
- **ESP32-S3 companion board** → communication, expansion, debugging, and support functions

This gives me a cleaner system architecture and more flexibility as the project grows.

## Design Focus for v1.0
For Version 1.0, the focus was on:

- Building a clean first-pass board architecture
- Integrating the core ESP32-S3 support hardware
- Adding modular expansion interfaces
- Making firmware flashing and bring-up easier
- Creating a platform that can be improved in future revisions

This version is primarily about getting the **hardware foundation** in place.

---

## Future Plans
This board is still in its early stages, and future revisions will likely include both electrical and firmware improvements.

### Planned Next Steps
- Order and assemble the first revision of the board
- Perform initial bring-up and power validation
- Verify USB-C power and 3.3V regulation
- Test programming/debug functionality with ESP-PROG
- Bring up onboard LEDs, switches, and sensor interfaces
- Validate I2C and SPI expansion functionality

### Long-Term Plans
- Pair this board with a **custom STM32 flight controller**
- Use it as part of a full **autonomous drone electronics stack**
- Add communication between the ESP32-S3 and STM32
- Expand support for telemetry and external peripherals
- Potentially integrate Ethernet or other network-capable modules for development and testing
- Continue revising the board based on testing and system needs


---

## Version
**Current Version:** `v1.0`

This is the first revision of the board and is intended to serve as the initial hardware foundation for future testing and iteration.

---

## Author
Designed and developed by me as part of my long-term embedded systems / autonomous drone project.

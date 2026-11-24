---
layout: post
title: "Diesel Heater Controller"
date: 2026-11-09
order: 11
image: "/assets/img/projects/diesel-heater-front.png"
---

A modular ESP32 controller for diesel heaters with serial bus interfacing, HC-05 Bluetooth remote phone control, I2C OLED display, and 1-wire digital temperature sensing.

<!--more-->

I designed a controller board for diesel heaters, based on an ESP32 module. A serial communication interface connects it to the heater, so it can send commands and read the heater's status.

A temperature sensor connector takes a one-wire digital temperature probe, and an I2C OLED display shows the heater's status and settings. Push buttons let the user operate and configure the heater locally, while a Bluetooth module allows wireless remote control from a phone. A real time clock supports time based scheduling, and an EEPROM keeps user settings when the power is off.

An onboard voltage regulator powers everything from the heater's supply, and a debug port makes programming and testing easy. The board is split into a main controller board and a display and button board, so it can be fitted in a compact enclosure.

<img src="{{ '/assets/img/projects/diesel-heater-front.png' | relative_url }}" alt="Diesel Heater Controller Main Board 3D Render">

### Key Features

- **ESP32 controller** with dual-core processing
- **Serial communication interface** communicating with the diesel heater
- **HC-05 Bluetooth module** for wireless smartphone monitoring and control
- **I2C OLED display** and multi-button user control interface
- **One-wire digital temperature sensor** interface
- **Real-time clock (RTC) and EEPROM** for automated scheduling and persistent settings
- **Onboard wide-input voltage regulation** with dedicated programming/debug headers

<img src="{{ '/assets/img/projects/diesel-heater-back.png' | relative_url }}" alt="Diesel Heater OLED Display and Button Board 3D Render">


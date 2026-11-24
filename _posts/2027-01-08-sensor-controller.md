---
layout: post
title: "Sensor Controller"
date: 2027-01-08
order: 12
image: "/assets/img/projects/sensor-controller-render.png"
---

An industrial ESP32 automation controller reading flow, seed, and load cell weight sensors while controlling stepper motors and solenoids over CAN bus.

<!--more-->

An ESP32-based controller board for precision monitoring and automation. It reads flow, seed and weight sensors and drives a stepper motor and a solenoid, and it connects to other equipment over CAN.

A USB Type-C port with a USB to serial interface is used for programming and debugging. The board runs from 12 V and 24 V inputs with fuse protection. Onboard regulators generate the 12 V, 8 V, 5 V and 3.3 V rails the peripherals need, and level shifters connect the 3.3 V controller to the 5 V sensor and driver signals. Indication LEDs, buttons and spare GPIO and analog inputs and outputs make the board easy to test and extend.

<img src="{{ '/assets/img/projects/sensor-controller-render.png' | relative_url }}" alt="Precision Sensor and Motion Controller PCB 3D Render">

### Key Features

- **ESP32 controller** for industrial automation
- **USB Type-C** with integrated USB-to-serial interface
- **CAN bus interface** for machine-to-machine industrial networking
- **Load cell instrumentation amplifier** for high-precision weight measurement
- **Flow sensor and optical seed sensor** interfaces
- **Integrated stepper motor driver** and power solenoid driver
- **Multi-rail power delivery:** 12 V, 8 V, 5 V, and 3.3 V regulated rails
- **Bidirectional level shifting** between 3.3 V logic and 5 V field signals
- **Dual 12 V and 24 V power inputs** with automotive fuse protection


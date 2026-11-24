---
layout: post
title: "Motor Controller PCB Reverse Engineering"
date: 2026-11-14
order: 6
image: "/assets/img/projects/motor-controller-render.png"
---

Reverse engineering and modernization of an obsolete boat motor control board into KiCad, featuring an MC68HC711E9 MCU, full-bridge motor driver, and isolated feedback.

<!--more-->

I reverse engineered an obsolete boat motor control board and rebuilt its design in KiCad, with a full schematic, PCB layout and BOM. The board is built around an MC68HC711E9 microcontroller.

It drives a DC motor through a full-bridge motor driver with current sensing, and uses an isolated feedback stage for signal sensing. Relay outputs switch the motor and clutch and select between main and backup operation. A 24 V input feeds 12 V and 5 V regulators, and a backup power path keeps the board running. It also has an RPM input with comparator conditioning, local and remote control inputs, main and backup alarm outputs, fuse and surge protection, and a reset supervisor.

I checked all connections against the original board and replaced obsolete parts with modern, readily available equivalents.

<img src="{{ '/assets/img/projects/motor-controller-render.png' | relative_url }}" alt="Rebuilt Motor Controller PCB 3D Render in KiCad">

### Key Features

- **MC68HC711E9** microcontroller core
- **Full-bridge DC motor driver** with real-time current sensing
- **Isolated feedback stage** for noise immunity
- **Main and backup relays** for motor, clutch, and system switching
- **24 V input** with dual 12 V and 5 V regulators and backup power path
- **RPM input** with analog comparator conditioning
- **Comprehensive protection:** input fuse, surge clamping, and power-on reset supervisor


---
layout: post
title: "I/O Controller"
date: 2026-11-16
order: 4
image: "/assets/img/projects/io-controller-render.png"
---

An industrial I/O controller PCB for remote monitoring and control of digital signals, featuring an AVR128DB48 MCU, W5500 Ethernet, and isolated RS485.

<!--more-->

I designed an I/O controller PCB for remote monitoring and control of digital signals. An AVR128DB48 microcontroller reads 14 digital inputs and drives 7 digital outputs.

For communication, a W5500-based Ethernet interface connects it to a local network, and an RS485 port supports wired serial links over longer distances and in noisy environments. Onboard voltage regulators provide the supply rails for the logic and interfaces.

<img src="{{ '/assets/img/projects/io-controller-render.png' | relative_url }}" alt="Numen Hub I/O Controller 3D Render">

### Key Features

- **AVR128DB48** microcontroller
- **14 digital inputs** and **7 digital outputs**
- **Ethernet** connectivity via W5500
- **RS485** serial interface for robust industrial field communications
- **Onboard voltage regulation** and protection circuitry

<img src="{{ '/assets/img/projects/io-controller-assembled.jpeg' | relative_url }}" alt="Numen Hub I/O Controller Assembled Hardware">


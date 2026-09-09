---
layout: post
title: "Level 2 EV Charger Controller Board"
date: 2026-09-01
---

A 4-layer EV charger controller board designed in KiCad, built around an
STM32 microcontroller with a pluggable microprocessor module.

<!--more-->

<img src="{{ '/assets/img/projects/ev-charger-render.png' | relative_url }}" alt="Level 2 EV charger controller board — 3D render">

## Overview

- **MCU:** STM32 (main), pluggable microprocessor module
- **Interfaces:** Ethernet, USB, Power-over-RS485, CAN, and serial (UART)
- **Safety:** Ground Fault Interrupter (GFI) and Protective Earth Neutral
  (PEN) fault detection circuits
- **Layers:** 4
- **Tools:** KiCad, oscilloscope, logic analyzer, multimeter

## Details

The board integrates Ethernet, USB, Power-over-RS485, CAN, and serial
communication interfaces for robust connectivity, alongside the GFI and PEN
detection circuits required for safe operation. The stack-up was optimized
for signal integrity, reduced EMI, and efficient power distribution —
built to be a smart, flexible, and safe controller for modern Level 2 EV
charging stations.

<img src="{{ '/assets/img/projects/ev-charger-layout.png' | relative_url }}" alt="Level 2 EV charger controller board — PCB layout in KiCad">

This work was carried through as part of the main controller PCB design at
Vega Innovations, covering IPC-compliant layout, BOM optimization for DFM,
and hardware verification against the J1772 charging protocol.

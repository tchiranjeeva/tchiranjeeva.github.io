---
layout: post
title: "RGB LED Controller Using Power over RS485"
date: 2026-08-27
---

A compact 4-layer PCB for controlling WS2812 addressable RGB LEDs using
Power over RS485 — power delivery and data communication over a single
2-wire bus.

<!--more-->

<img src="{{ '/assets/img/projects/rs485-led-render1.png' | relative_url }}" alt="RGB LED controller board — top view">

## Overview

- **MCU:** STM32G030F6P6
- **Link:** Isolated RS485 (power + data over 2 wires)
- **Load:** WS2812 addressable RGB LED strip
- **Power:** Onboard 12 V → 5 V / 3.3 V regulation
- **Layers:** 4
- **Extras:** Buzzer output, protection circuitry

## Details

The design carries both power and data to the LED strip over a single
RS485 pair, with onboard regulation stepping the incoming 12 V down to the
5 V and 3.3 V rails the board needs. It includes an isolated RS485
transceiver stage, buzzer output, and protection circuitry for reliable
operation in an industrial setting. The layout was optimized for signal
integrity and EMI performance, making it suitable for long-distance LED
installations and distributed lighting applications.

<img src="{{ '/assets/img/projects/rs485-led-layout.png' | relative_url }}" alt="RGB LED controller board — PCB layout in KiCad">
<img src="{{ '/assets/img/projects/rs485-led-render2.png' | relative_url }}" alt="RGB LED controller board — angled render">

---
layout: post
title: "Diesel Heater Controller"
date: 2026-09-08
---

A controller PCB for diesel heaters built around an ESP32, with Bluetooth
remote control and an onboard display for real-time status.

<!--more-->

<img src="{{ '/assets/img/projects/diesel-heater-front.png' | relative_url }}" alt="Diesel heater controller board — front side render">

## Overview

- **MCU:** ESP32
- **Connectivity:** Bluetooth module for remote control
- **Display:** I2C display for real-time status monitoring
- **Storage & timing:** EEPROM for user settings, RTC module for time-based scheduling
- **Input:** Button switches for manual operation

## Details

Combines an ESP32 for processing and wireless connectivity with a Bluetooth
module for remote operation, alongside physical buttons for manual control
when needed. The I2C display gives real-time status feedback, while the
EEPROM and RTC handle persistent settings and scheduled operation — a
compact, user-friendly layout aimed at controlling diesel heaters reliably.

<img src="{{ '/assets/img/projects/diesel-heater-back.png' | relative_url }}" alt="Diesel heater controller board — display and button side render">
<img src="{{ '/assets/img/projects/diesel-heater-layout.png' | relative_url }}" alt="Diesel heater controller board — PCB layout">

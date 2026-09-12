---
layout: post
title: "Sensor Controller"
date: 2026-09-05
---

An ESP32-based sensor control PCB for intelligent monitoring and
automation, with multiple regulated power rails and CAN communication.

<!--more-->

<img src="{{ '/assets/img/projects/sensor-controller-render.png' | relative_url }}" alt="Sensor controller board render">

## Overview

- **MCU:** ESP32
- **Power rails:** 12 V, 8 V, 5 V, 3.3 V (regulated onboard)
- **Programming:** USB Type-C
- **Communication:** CAN
- **I/O:** Flow and seed sensors, stepper motor driver, solenoid driver,
  load cell amplifier

## Details

A compact, versatile board aimed at precision control and data
acquisition — the multiple regulated rails let it directly power a mix of
sensors and actuators (flow/seed sensors, a stepper driver, a solenoid
driver, a load cell amplifier) without external supplies, while CAN gives
it a robust link into a larger control network.

<img src="{{ '/assets/img/projects/sensor-controller-layout.png' | relative_url }}" alt="Sensor controller board — PCB layout in KiCad">

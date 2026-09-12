---
layout: post
title: "IoT Controller (Stratus Log)"
date: 2026-08-22
---

A 4-layer industrial IoT controller for remote environmental monitoring and
data acquisition, built around an ATmega1284P.

<!--more-->

<img src="{{ '/assets/img/projects/iot-controller-render.png' | relative_url }}" alt="IoT controller board — render">

## Overview

- **MCU:** ATmega1284P
- **Wireless:** LSM100A LoRa/Sigfox module for long range communication
- **Storage & timing:** microSD data logging, DS3231M RTC with backup battery
- **Power input:** 5–15 V, with onboard 3.3 V, 5 V, and 12 V regulation
- **I/O:** SDI-12 sensor interface, Schmitt trigger conditioned pulse input,
  pluggable screw terminals, ESD protection
- **Layers:** 4

## Details

Built as a modular, field-deployable controller for remote monitoring
the SDI-12 interface and pulse input cover common environmental sensors,
while the LoRa/Sigfox module handles long range backhaul where cellular or
Wi-Fi isn't practical. Multiple regulated rails and a wide 5-15 V input
range make it easy to power from solar or battery systems in the field.

<img src="{{ '/assets/img/projects/iot-controller-layout.png' | relative_url }}" alt="IoT controller board — PCB layout in KiCad">

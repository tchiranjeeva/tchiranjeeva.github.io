---
layout: post
title: "Equine Wearable Tracker"
date: 2026-08-18
---

A compact 4-layer wearable PCB for equine health and location monitoring,
built around an nRF52840 SoC.

<!--more-->

<img src="{{ '/assets/img/projects/equine-tracker-render.png' | relative_url }}" alt="Equine wearable tracker board — render">

## Overview

- **SoC:** nRF52840 (Bluetooth Low Energy)
- **GNSS:** MAX-M10S for real-time GPS tracking
- **Motion sensing:** BMI270 IMU + BMM350 magnetometer
- **Storage:** 128 Mb SPI flash for data logging
- **Physiological monitoring:** AD8232 ECG front end
- **Power:** Li-ion charging and power management, USB connectivity
- **Layers:** 4

## Details

The tracker combines location (GNSS), motion (IMU + magnetometer), and
physiological sensing (ECG front end) in a single wearable board, with
onboard flash for logging and Li-ion charge management for long field use.
Antenna matching networks and low-power circuit design were priorities
throughout, given the battery-life constraints of a wearable device.

<img src="{{ '/assets/img/projects/equine-tracker-layout.png' | relative_url }}" alt="Equine wearable tracker board — PCB layout in KiCad">

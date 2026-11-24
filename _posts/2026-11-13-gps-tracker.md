---
layout: post
title: "GPS Tracker"
date: 2026-11-13
order: 7
image: "/assets/img/projects/equine-tracker-render.png"
---

A miniature wearable tracker for equine monitoring, built with an nRF52840 BLE SoC, MAX-M10S GNSS, 9-DOF IMU/magnetometer, AD8232 ECG, and onboard flash logging.

<!--more-->

I designed a small wearable tracker for equine monitoring, built around an nRF52840 microcontroller with Bluetooth Low Energy. A MAX-M10S GNSS receiver provides real-time location.

A BMI270 IMU and a BMM350 magnetometer capture motion and orientation. An AD8232 ECG front end measures heart activity. A 128 Mb W25Q128JV flash chip stores data on the device, and a Li-Po charging circuit, voltage regulation and USB connection take care of power and charging. I designed the antenna layouts for both the Bluetooth radio and the GNSS receiver using ceramic antennas.

<img src="{{ '/assets/img/projects/equine-tracker-render.png' | relative_url }}" alt="Wearable Equine GPS Tracker PCB 3D Render">

### Key Features

- **nRF52840** SoC with Bluetooth Low Energy (BLE)
- **MAX-M10S GNSS** receiver for real-time positioning
- **BMI270 6-axis IMU** and **BMM350 magnetometer** for motion & gait capture
- **AD8232 analog front end** for ECG and heart rate measurement
- **128 Mb SPI flash** for autonomous offline telemetry logging
- **Integrated Li-Po charger**, power management, and USB interface
- **Dual ceramic antennas** tuned for BLE and satellite GNSS reception


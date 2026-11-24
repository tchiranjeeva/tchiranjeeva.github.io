---
layout: post
title: "BLE Beacon"
date: 2026-11-07
order: 13
image: "/assets/img/projects/ble-beacon-front.png"
---

An ultra-compact, coin-cell battery powered Bluetooth Low Energy beacon built on an nRF52840 module with a low-power accelerometer for motion wake-up interrupts.

<!--more-->

A compact, battery powered Bluetooth Low Energy beacon built around an nRF52840 based wireless module. A low power accelerometer connects to the microcontroller over I2C and sends an interrupt signal when it detects motion, so the beacon can wake up and react to movement.

The board runs from a coin cell battery in an onboard holder, with a slide switch to turn it on and off. A programming and debug header gives access to the microcontroller for firmware upload and testing, and mounting holes allow the board to be fixed in an enclosure or on an asset.

<img src="{{ '/assets/img/projects/ble-beacon-front.png' | relative_url }}" alt="nRF52840 BLE Beacon Top View 3D Render">

### Key Features

- **nRF52840-based Bluetooth Low Energy** wireless module
- **Ultra-low power I2C accelerometer** with configurable motion interrupt wake-up
- **CR2032 coin cell battery** with surface-mount onboard holder
- **Sub-miniature slide power switch**
- **SWD programming and debug header** for firmware flash and debugging
- **Integrated mounting holes** for quick enclosure and asset attachment
- **Minimal component count** optimized for maximum battery life

<img src="{{ '/assets/img/projects/ble-beacon-back.png' | relative_url }}" alt="BLE Beacon Bottom View with Coin Cell Holder">


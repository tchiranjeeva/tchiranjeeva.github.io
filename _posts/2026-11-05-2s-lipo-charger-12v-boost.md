---
layout: post
title: "2S Li-Po Charger and 12V Boost Converter"
date: 2026-11-05
order: 15
image: "/assets/img/projects/2s-lipo-charger-boost-render.png"
---

A compact 4-layer power board charging 2-cell (2S) Li-Po batteries from USB Type-C with balanced cell management and boosting voltage to a regulated 12V output.

<!--more-->

A compact power board that charges a 2 cell (2S) Li-Po battery from USB Type-C and boosts the battery voltage to a regulated 12 V output. A dedicated charger IC handles balanced charging, so both cells stay at the same voltage, and it can be configured and monitored over I2C.

An NTC thermistor monitors the battery temperature, and a fuse protects the input. A high efficiency boost converter then steps the battery voltage up to a stable 12 V, so the board can power 12 V devices such as routers and small electronics from a portable battery. The board is a 4-layer design, for good signal integrity, power distribution and thermal performance.

<img src="{{ '/assets/img/projects/2s-lipo-charger-boost-render.png' | relative_url }}" alt="2S Li-Po Charger and 12V Boost Converter 3D Render">

### Key Features

- **USB Type-C power input** with standard 5V charging
- **2-cell (2S) Li-Po balance charging** for cell longevity and safety
- **I2C communication interface** for charger configuration and telemetry
- **NTC thermistor sensing** for battery thermal protection
- **Input fuse protection**
- **High-efficiency synchronous boost converter** with regulated 12 V barrel jack output
- **4-layer KiCad PCB layout** with continuous ground planes and thermal vias


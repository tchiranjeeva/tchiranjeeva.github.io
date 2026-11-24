---
layout: post
title: "Power Distribution Board"
date: 2026-11-11
order: 9
image: "/assets/img/projects/power-distribution-render.png"
---

A compact 4-layer power distribution board for an underwater ROV, handling 4S LiPo power, reverse polarity protection, 6 ESC outputs, and I2C power telemetry.

<!--more-->

I designed a compact 4-layer power distribution board for an ROV (remotely operated underwater vehicle). It takes power from a 4S LiPo battery (14.8 V) and shares it across the vehicle's systems.

Reverse polarity and surge protection at the input guard the electronics against wiring mistakes and voltage spikes. The board supplies six ESCs for the thrusters and a switched LED lighting array, and a regulated 5 V rail powers the onboard Raspberry Pi and a PWM controller module. A built in telemetry circuit measures battery voltage and current, and the readings go to the Raspberry Pi over I2C so the vehicle's power use can be monitored in real time.

<img src="{{ '/assets/img/projects/power-distribution-layout.png' | relative_url }}" alt="ROV Power Distribution Board PCB Layout in KiCad">

### Key Features

- **4S LiPo (14.8 V) input** via high-current XT90 connector
- **Reverse polarity and transient (TVS)** surge protection
- **Six XT30 outputs** for brushless thruster ESCs
- **MOSFET-switched LED lighting output**
- **High-efficiency 5 V buck regulator** powering Raspberry Pi and PCA9685 PWM controller
- **INA226 voltage and current telemetry** monitored over I2C
- **4-layer KiCad design** optimized for heavy current copper planes and thermal dissipation

<img src="{{ '/assets/img/projects/power-distribution-render.png' | relative_url }}" alt="ROV Power Distribution Board 3D Render">


---
layout: post
title: "Stratus Logger"
date: 2026-11-12
order: 8
image: "/assets/img/projects/stratus-logger-render.png"
---

A rugged remote data logger powered by an ATmega1284P MCU, featuring Schmitt trigger rain gauge pulse counting, 16-bit ADC, microSD logging, and LoRa/Sigfox (868 MHz).

<!--more-->

I designed the Stratus Logger as a remote data logger built around an ATmega1284P microcontroller. A pulse input with Schmitt trigger conditioning counts the pulses from a tipping bucket rain gauge cleanly, even with slow or noisy edges.

A 16-bit ADC reads analog sensors, and a real time clock with a backup battery timestamps every reading, even if the main power is lost. Data is stored on a microSD card and sent through an LSM100A LoRa/Sigfox module (868 MHz), so the logger can report from sites with no Wi-Fi or mobile coverage. Onboard voltage regulators power the logic, radio and sensors from a wide input range.

<img src="{{ '/assets/img/projects/stratus-logger-render.png' | relative_url }}" alt="Stratus Remote Environmental Logger 3D Render">

### Key Features

- **ATmega1284P** microcontroller with ample flash and RAM
- **LSM100A LoRa / Sigfox module** (868 MHz) for long-range remote telemetry
- **Schmitt trigger pulse conditioning** for tipping bucket rain gauges
- **Precision 16-bit ADC** for environmental analog instrumentation
- **microSD card storage** for non-volatile local data backup
- **RTC with coin cell backup battery** for continuous timestamping
- **Wide input voltage regulation** providing multiple clean rails (12V, 5V, 3.3V)


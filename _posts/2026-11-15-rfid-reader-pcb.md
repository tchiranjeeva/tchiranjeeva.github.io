---
layout: post
title: "RFID Reader PCB"
date: 2026-11-15
order: 5
image: "/assets/img/projects/rfid-reader-render.png"
---

A compact 13.56 MHz RFID reader board with an etched PCB antenna coil, ATmega32U4 MCU, USB Type-C, adaptive ambient light sensor (LDR), and status LED ring.

<!--more-->

A compact RFID reader board with USB connectivity. A 13.56 MHz RFID reader IC reads contactless cards and tags through a printed antenna etched directly into the PCB. I designed the antenna coil and its matching network to give a reliable read range, so the board needs no external antenna part.

An ATmega32U4 microcontroller handles the reader and communicates with a host over USB Type-C, so it works as a plug in reader. A ring of LEDs around the antenna shows the reader's status, and a light dependent resistor (LDR) in the centre measures the ambient light so the LED brightness can adapt to the surroundings. A buzzer gives audible feedback on each read. A 3.3 V regulator powers the reader IC, and a programming header allows firmware updates and debugging.

<img src="{{ '/assets/img/projects/rfid-reader-render.png' | relative_url }}" alt="RFID Reader PCB 3D Render Front and Back">

### Key Features

- **13.56 MHz RFID reader** with custom etched PCB coil antenna and tuned matching network
- **ATmega32U4 microcontroller** with native USB support
- **USB Type-C** connection for power and communication
- **LED ring** for visual status indication
- **Ambient light sensor (LDR)** for automatic LED brightness adjustment
- **Buzzer** for audible feedback upon successful card read

<img src="{{ '/assets/img/projects/rfid-reader-assembled.png' | relative_url }}" alt="RFID Reader Fabricated and Assembled PCB">


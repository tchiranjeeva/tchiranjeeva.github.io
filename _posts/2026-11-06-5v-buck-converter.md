---
layout: post
title: "5V Buck converter"
date: 2026-11-06
order: 14
image: "/assets/img/projects/5v-buck-converter-render.png"
---

A compact step-down (buck) converter stepping 9–15V battery inputs down to a regulated 5V output at up to 8A, with MOSFET reverse polarity and TVS transient protection.

<!--more-->

A compact step down (buck) converter module that turns a 9-15 V battery or supply into a regulated 5 V output at up to 8 A. It is designed to power high current loads such as single board computers, cameras and other electronics from a 12 V battery.

The input stage is protected by a fuse, a TVS diode against voltage spikes, and a MOSFET based reverse polarity protection circuit, so the module and the load are safe if the battery is connected the wrong way or the supply has transients. Low ESR ceramic capacitors on the input and output keep the output voltage stable and the ripple low. Test points for the battery input, the 5 V output and ground make testing and measurement straightforward.

<img src="{{ '/assets/img/projects/5v-buck-converter-render.png' | relative_url }}" alt="5V 8A High-Current Buck Converter Module 3D Render">

### Key Features

- **Wide input range:** 9–15 V DC
- **High current output:** 5 V regulated at up to 8 A continuous
- **Automotive-grade input fuse**
- **High-speed TVS diode** for transient voltage surge clamping
- **Low-loss P-channel MOSFET** reverse polarity protection circuit
- **Low ESR ceramic input and output capacitors** for minimal ripple
- **Dedicated test points** for Vin, Vout, and GND validation


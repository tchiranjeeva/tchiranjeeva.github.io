---
layout: post
title: "Power Distribution Board"
date: 2026-09-04
---

A compact power distribution board for a 4S LiPo system, with fused ESC
outputs and onboard current/voltage monitoring.

<!--more-->

<img src="{{ '/assets/img/projects/power-distribution-render.png' | relative_url }}" alt="Power distribution board render">

## Overview

- **Input:** XT90 (4S LiPo)
- **Outputs:** Fused XT30 outputs for ESCs
- **Extras:** MOSFET-controlled lighting circuit, regulated 5 V output for
  a Raspberry Pi
- **Monitoring:** INA226 current/voltage interface
- **Layers:** 4

## Details

Designed as the central power hub for a 4S LiPo-powered system —
distributing fused power to multiple ESCs, switching accessory lighting
through a MOSFET stage, and stepping down a clean 5 V rail for a Raspberry
Pi, all while an INA226 keeps real-time current and voltage telemetry
available to the rest of the system.

<img src="{{ '/assets/img/projects/power-distribution-layout.png' | relative_url }}" alt="Power distribution board — PCB layout in KiCad">

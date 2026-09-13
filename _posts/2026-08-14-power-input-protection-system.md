---
layout: post
title: "Power Input Protection System"
date: 2026-08-10
---

A 6-layer protection PCB built for adverse electrical conditions
surge protection, PEN fault protection, and earth connectivity detection.

<!--more-->

<img src="{{ '/assets/img/projects/power-input-pcb-layout.png' | relative_url }}" alt="power input protection board — 3D render">

<img src="{{ '/assets/img/projects/mov-pcb-render.png' | relative_url }}" alt="surge protection board — 3D render">

## Overview

- **Layers:** 6
- **Protections:** Surge protection, PEN (Protective Earth Neutral) fault
  detection, earth connectivity detection
- **Tools:** KiCad, hipot tester, oscilloscope, variac, multimeter

## Details

A 3-phase power input protection system designed for EV chargers to improve electrical safety and reliability. The latest version uses a two board stacked PCB architecture: the main board handles the 3-phase power input and protection/control circuitry, while a dedicated protection board carries four isolated MOVs and a GDT for surge protection.

The design also integrates PEN fault protection, earth connectivity detection, and an onboard SMPS, providing protection against surges, grounding faults, and other electrical hazards. Both boards are designed as a 6-layer PCBs with careful isolation and layout considerations for high voltage power applications.

<img src="{{ '/assets/img/projects/power-input-pcb-render.png' | relative_url }}" alt="protection pcb stack">
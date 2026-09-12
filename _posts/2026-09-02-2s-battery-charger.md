---
layout: post
title: "2S Battery Charger"
date: 2026-09-02
---

A 4-layer Li-Po battery charger and boost converter board with USB-C power
delivery input and a regulated 12 V boost output.

<!--more-->

<img src="{{ '/assets/img/projects/2s-battery-charger-render.png' | relative_url }}" alt="2S battery charger board render">

## Overview

- **Input:** USB Type-C, power delivery
- **Charging:** 2-cell (2S) Li-Po balance charging with safety protection
- **Output:** High-efficiency boost converter, regulated 12 V
- **Layers:** 4

## Details

Takes USB-C power delivery in and handles balanced charging across two
Li-Po cells, with the usual protection circuitry to keep that safe. A
high-efficiency boost stage then steps the battery's output up to a
regulated 12 V rail, making the board double as both a charger and a
portable 12 V power source. The 4-layer stack-up was chosen for better
signal integrity, power distribution, and thermal performance in a compact
footprint.

<img src="{{ '/assets/img/projects/2s-battery-charger-layout.png' | relative_url }}" alt="2S battery charger board — PCB layout in KiCad">

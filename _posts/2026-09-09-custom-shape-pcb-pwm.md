---
layout: post
title: "Custom Shape PCB for PWM Generation"
date: 2026-09-09
---

A custom-shaped 4-layer add-on PCB designed to solder directly onto an
existing piece of hardware using castellated holes.

<!--more-->

<img src="{{ '/assets/img/projects/custom-shape-pcb-photo.png' | relative_url }}" alt="Custom shape PCB for PWM generation — assembled board photo">

## Overview

- **Layers:** 4
- **Form factor:** Custom outline, shaped to fit an existing hardware item
- **Mounting:** Castellated holes for direct soldering onto existing pins
- **Tools:** KiCad

## Details

Rather than a standalone board, this was designed as an add-on that
solders directly onto an existing piece of hardware to extend its
functionality — generating PWM signals for it. The castellated holes along
the board edge let it solder cleanly and reliably onto the host hardware's
existing pins, and the outline was custom-shaped to fit the available
space rather than using a standard rectangular board.

<img src="{{ '/assets/img/projects/custom-shape-pcb-layout.png' | relative_url }}" alt="Custom shape PCB for PWM generation — PCB layout in KiCad">
<img src="{{ '/assets/img/projects/custom-shape-pcb-assembled.png' | relative_url }}" alt="Custom shape PCB for PWM generation — mounted on host hardware">

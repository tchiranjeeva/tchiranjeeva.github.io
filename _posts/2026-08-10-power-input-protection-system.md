---
layout: post
title: "Power Input Protection System"
date: 2026-08-10
---

A 6-layer protection PCB built for adverse electrical conditions —
surge protection, PEN fault protection, and earth connectivity detection.

<!--more-->

## Overview

- **Layers:** 6
- **Protections:** Surge protection, PEN (Protective Earth Neutral) fault
  detection, earth connectivity detection
- **Tools:** KiCad, hipot tester, oscilloscope, variac, multimeter

## Details

Implements fault detection algorithms to keep the connected system safe
under surge events and earth/neutral faults — the kind of protection stage
that sits ahead of sensitive downstream electronics in equipment like EV
chargers. Validated on the bench with a hipot tester and variac to confirm
behavior under simulated fault and overvoltage conditions.

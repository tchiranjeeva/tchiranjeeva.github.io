---
layout: post
title: "Network Controller Module"
date: 2026-07-28
---

A compact, pluggable, modular 4-layer PCB integrating a microprocessor and
4G connectivity for IoT applications.

<!--more-->

<img src="{{ '/assets/img/projects/network-controller-render.jpg' | relative_url }}" alt="network controller render">

## Overview

- **Layers:** 4
- **Connectivity:** 4G communication module with integrated antenna, SIM
  card interface
- **Interfaces:** RS485, USB hub
- **Form factor:** Compact, pluggable module
- **Tools:** Eagle, Fusion 360

## Details

Built as a plug in module rather than a fixed board, so the 4G/RS485/USB
stack can be dropped into different host systems. The integrated antenna
4G module and SIM interface handle cellular backhaul, while the USB hub and
RS485 port give it a physical and serial connection to local peripherals.

<img src="{{ '/assets/img/projects/network-controller-layout.png' | relative_url }}" alt="network controller — PCB layout in Eagle">

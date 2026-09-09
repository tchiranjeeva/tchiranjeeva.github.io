---
layout: post
title: "Real-Time Energy Monitoring System"
date: 2026-07-12
---

An STM32-based energy measurement solution using SWV tracing for
real-time voltage/current waveform visualization.

<!--more-->

## Overview

- **MCU:** STM32 (STM32CubeIDE)
- **Debug/visualization:** SWV (Serial Wire Viewer) tracing
- **Tools:** multimeter

## Details

Uses STM32CubeIDE's SWV tracing to visualize voltage and current waveforms
in real time while the firmware computes energy consumption — useful for
verifying the measurement pipeline against a bench multimeter without
needing a separate data-logging setup.

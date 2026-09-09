---
layout: post
title: "Thermal Protection Device"
date: 2026-08-05
---

A 4-layer PCB for a thermal safety device designed to prevent electrical
fires, using dual NTC thermistors and relay-based AC isolation.

<!--more-->

## Overview

- **Layers:** 4
- **Sensing:** Dual NTC thermistors, analog comparator
- **Protection logic:** Latch circuit, relay-based AC isolation
- **Indicators:** Adjustable temperature thresholds, LED indicators, buzzer alert
- **Tools:** KiCad, oscilloscope, multimeter, LTspice

## Details

Dual thermistors feed an analog comparator stage that trips a latch circuit
once a temperature threshold is exceeded, isolating the AC load through a
relay. Thresholds are adjustable, with LED and buzzer feedback so a fault
condition is immediately visible — a small, self-contained safety layer
that can sit in front of any AC load prone to overheating.

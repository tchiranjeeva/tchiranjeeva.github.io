---
layout: post
title: "LED Controller Board"
date: 2026-09-07
---

A 2-layer controller board for a flexible LED strip, built around an ESP32
with USB-C for both firmware upload and battery charging.

<!--more-->

<img src="{{ '/assets/img/projects/led-controller-board.png' | relative_url }}" alt="LED controller board render">

## Overview

- **MCU:** ESP32
- **Layers:** 2
- **Power:** USB Type-C (firmware upload + charging), single-cell Li-ion
  charging, 5 V boost for portable operation
- **Extras:** USB-to-serial converter and level shifter onboard

## Details

Built for wireless control and advanced lighting effects on a flexible LED
strip. The USB-C port does double duty — flashing firmware and charging
the onboard Li-ion cell — with a boost converter stepping the battery
voltage up to a stable 5 V for portable operation away from mains power.
The onboard USB-to-serial converter and level shifter keep development and
debugging straightforward without extra hardware.

---
layout: post
title: "Linear Voltage Regulators"
date: 2026-11-01
order: 19
image: "/assets/img/projects/linear-regulator-v1.png"
---

Two precision benchtop adjustable linear power supplies engineered for sensitive analog and microcontroller testing, featuring low noise, external pass transistors, and current limiting.

<!--more-->

I designed two adjustable linear power supplies for the electronics bench. Each takes an AC input and rectifies and smooths it into a DC supply. A linear regulator stage with a power transistor then provides a stable, low-noise output, and potentiometers let the user set the output voltage and the current limit.

The first version builds the regulation around an adjustable linear regulator IC and an external pass transistor for higher current. The second version uses an op-amp feedback loop with a precision reference and a current sense resistor, and it brings out voltage and current signals to drive a display. Both have an input fuse for protection and a status LED, and they are laid out for heat sinking of the power devices. Linear regulation gives clean, quiet power, which suits sensitive analog and microcontroller testing.

<img src="{{ '/assets/img/projects/linear-regulator-v1.png' | relative_url }}" alt="Benchtop Linear Voltage Regulator Version 1 with TO-3 Transistor">

### Key Features

- **AC-to-DC rectification and heavy capacitive smoothing**
- **Version 1:** Linear regulator IC with external TO-3 pass transistor for boosted load current
- **Version 2:** Precision op-amp feedback control with low-drift voltage reference and current sense
- **Independent potentiometer adjustments** for fine output voltage and current limit setting
- **Auxiliary telemetry outputs** for digital panel meter integration
- **Fused protection**, status indication, and dedicated power heatsink layout
- **Ultra-low output ripple and noise** ideal for sensitive RF and analog debugging

<img src="{{ '/assets/img/projects/linear-regulator-v2.png' | relative_url }}" alt="Benchtop Linear Voltage Regulator Version 2 with Op-Amp Control and Heatsinks">


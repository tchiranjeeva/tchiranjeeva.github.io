---
layout: post
title: "Energy Management System (EMS)"
date: 2026-11-18
order: 2
image: "/assets/img/projects/ems-controller-top.png"
---

An Energy Management System (EMS) controller PCB for EV charging hubs, coordinating multiple chargers and linking the site to the cloud with Wi-Fi, cellular, and energy metering.

<!--more-->

I designed an Energy Management System (EMS) controller PCB for EV charging hubs. It sits at the centre of the hub, coordinating the chargers and linking the site to the cloud. An ESP32 provides Wi-Fi, which is the main link because the EMS and chargers share the same network. Where Wi-Fi isn't available, a 4G or LoRa module can be added through the onboard mini PCIe slot. Chargers and other devices can also be wired to the EMS over RS485 or CAN.

An onboard energy meter module measures the power entering the charging bay. The board is powered by its own AC-DC supply with DC voltage regulators, and a battery backup supports low-power operation. For local use, it has an OLED display with buttons, a buzzer, and two relay outputs.

<img src="{{ '/assets/img/projects/ems-controller-top.png' | relative_url }}" alt="Energy Management System (EMS) PCB Top View">

### Key Features

- **ESP32 controller** with Wi-Fi as the primary link
- **Mini PCIe slot** for an optional 4G or LoRa module
- **RS485 and CAN** for wired charger and device connections
- **Energy meter module** for bay input power monitoring
- **AC-DC supply**, DC regulators, and battery backup
- **OLED display** with buttons, buzzer, and two relay outputs

**Current Status:** Hardware Tested & Verified

<img src="{{ '/assets/img/projects/ems-controller-assembled.png' | relative_url }}" alt="Energy Management System Assembled with 18650 Battery and Display">


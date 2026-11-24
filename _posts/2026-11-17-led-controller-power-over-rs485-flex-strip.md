---
layout: post
title: "LED Controller with Power over RS485 + Flex LED Strip"
date: 2026-11-17
order: 3
image: "/assets/img/projects/rs485-led-controller-board.jpg"
---

A compact LED controller delivering both power and high-speed data over a single two-wire RS485 cable via a custom bias tee network, driving 172 LEDs across two flex strips.

<!--more-->

A compact LED controller that receives both power and data over a single two-wire RS485 cable. I designed the bias tee network that combines the DC supply with the RS485 signal on the same pair, and an SN65HVD11HD transceiver handles the data.

An STM32G030F6P6 microcontroller drives the LEDs through a level shifter (3.3 V to 5 V), and the board also includes voltage regulation and a buzzer output. I also designed the matching flex LED strip with 86 LEDs. Two strips connect to each controller, giving 172 LEDs per node.

<img src="{{ '/assets/img/projects/rs485-led-controller-board.jpg' | relative_url }}" alt="LED Controller Board with Power Over RS485">

### Key Features

- **Power and data over one RS485 pair** (bias tee network)
- **SN65HVD11HD** RS485 transceiver
- **STM32G030F6P6** microcontroller
- **74AHCT1G125** level shifter for the LED data line
- **Onboard voltage regulation** and buzzer output
- **Flex LED strip** with 86 LEDs (two strips per controller = 172 LEDs total)

<img src="{{ '/assets/img/projects/rs485-flex-led-strip.jpg' | relative_url }}" alt="Flexible LED Strip Connected to Controller">


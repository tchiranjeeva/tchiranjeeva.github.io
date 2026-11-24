---
layout: post
title: "Touch Controlled Flex LED Strip"
date: 2027-01-10
order: 10
image: "/assets/img/projects/flex-touch-controller-render.png"
---

An interactive lighting system featuring an ESP32-S3 rigid controller board with USB-C and LiPo charging, linked via FPC to an ultra-thin flex strip with capacitive touch sensors.

<!--more-->

I designed an interactive lighting system made of a rigid controller board and a flexible LED strip. The controller is built around an ESP32-S3 and has a USB Type-C port for power and programming, a USB-to-serial interface for firmware upload, and a LiPo battery charger with voltage regulation for portable use. A level shifter lifts the 3.3 V logic signal to the level the addressable RGB LEDs need.

The flex strip connects to the controller through an FPC connector. It carries the LEDs and a set of capacitive touch sensors. When someone touches the sensors, the lighting changes: the touch input switches the light pattern and adjusts the brightness and the animation speed. The flexible construction makes the strip light and thin, so it suits wearable and compact lighting applications.

<img src="{{ '/assets/img/projects/flex-touch-controller-render.png' | relative_url }}" alt="ESP32-S3 Rigid LED Controller Board 3D Render">

### Key Features

- **ESP32-S3 microcontroller** with native USB and wireless capabilities
- **USB Type-C port** with onboard USB-to-serial interface
- **LiPo battery management** with charging circuit and power path
- **High-speed level shifting** for 5V addressable RGB LED data lines
- **Ultra-thin Flexible PCB (Flex strip)** connecting via FPC cable
- **On-strip capacitive touch sensors** controlling animation, color, and brightness

<img src="{{ '/assets/img/projects/flex-touch-strip-render.png' | relative_url }}" alt="Capacitive Touch Flexible LED Strip 3D Render">


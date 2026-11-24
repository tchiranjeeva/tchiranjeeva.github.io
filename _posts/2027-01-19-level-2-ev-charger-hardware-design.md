---
layout: post
title: "Level 2 EV Charger Hardware Design"
date: 2027-01-19
order: 1
image: "/assets/img/projects/ev-charger-render.png"
---

A complete hardware suite designed for Level 2 EV charging stations: a main controller board, a pluggable network module, and power input and surge protection boards.

<!--more-->

A set of boards I designed for Level 2 EV charging stations: a main controller, a pluggable network module, and input power and protection boards.

**My Role:** Sole PCB designer from schematic to production files.

---

### 1.1 Level 2 EV Charger Controller Board

I designed the main controller board for a Level 2 EV charging station. An STM32 microcontroller runs the charging logic and manages the safety systems. The control pilot and proximity pilot circuits handle communication with the vehicle. They signal the available charging current and detect when the plug is connected.

A ground fault interrupter (GFI) circuit with an automatic self test, together with protective earth neutral (PEN) fault and earth connection detection, shuts the charger down when it senses an unsafe condition. The board drives the main contactor and a plug lock solenoid, and it can run an LED status strip, a buzzer and a button.

For connectivity, it provides Ethernet, CAN, RS485 and power over RS485, two USB outputs with current limiting, and a connector for a pluggable network controller module with a Linux processor. It runs from a 24 V input, with onboard regulators for the 12 V, 5 V and 3.3 V rails, and DIP switches let the installer set configuration options. The 4-layer layout is designed for signal integrity and low EMI.

<img src="{{ '/assets/img/projects/ev-charger-render.png' | relative_url }}" alt="Level 2 EV Charger Controller Board 3D Render">

<img src="{{ '/assets/img/projects/ev-charger-assembled.png' | relative_url }}" alt="Level 2 EV Charger Controller Assembled Board Stack">

---

### 1.2 Power Input Protection PCB

The input stage of a three-phase EV charger, designed to carry up to 32 A AC. It is a 6-layer PCB with 2 oz copper, with wide traces and copper pours that handle the full current. The three phases, neutral and earth come in through heavy-duty connectors and are protected by an input fuse.

An onboard AC-DC power supply produces the 24 V rail for the charger's electronics. The board also monitors the supply for safety faults. A PEN fault detection circuit detects a fault between the protective earth and neutral conductors, and an earth connection detection circuit checks that the ground connection is intact. Comparators and a current transformer feed these signals to the charger's microcontroller. When a fault is found, MCU-controlled relays switch the supply so the charger stops operating.

<img src="{{ '/assets/img/projects/power-input-pcb-photo.png' | relative_url }}" alt="Power Input Protection PCB Photo">

---

### 1.3 Surge Protection PCB

A surge protection board that sits at the input of the EV charger. Four varistors (MOVs), one for each of the three phases and the neutral, clamp voltage spikes caused by lightning or grid switching. A gas discharge tube (GDT) adds a second stage of protection by diverting very large surges to earth. Together, they keep the charger and the vehicle safe from overvoltage events.

<img src="{{ '/assets/img/projects/mov-pcb-render.png' | relative_url }}" alt="Surge Protection PCB 3D Render">


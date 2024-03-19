---
title: Drone Flight Control System Integration
type: blog
prev: blog/
sidebar:
  open: true
math: true
---

This blog post is still in the making...

## Introduction
I recently started designed a long-range drone system (from commercially available parts) for a control system integration project and to (hopefully) end up with a functioning drone at the end.

[Ardupilot](https://ardupilot.org) is an open-source software repository with various implementations of control systems for RC planes, drones, rovers, and more. The challenge I am currently battling is customising the Ardupilot-specific code to run on my Raspberry Pi Zero. 

## Hardware Stack

These are the critical systems onboard:
  - Airframe
  - Motors
  - Propellers
  - Battery pack
  - Camera system
  - Propeller controller
  - Communications antennas
  - Flight management and computers

### Airframe

Epoxy-carbon composite sheet-cut, X-frames seem a popular and affordable solution for medium-sized long range drones. I got one from [Aliexpress](https://www.aliexpress.com/item/1005006326462952.html?spm=a2g0o.order_list.order_list_main.11.7a291802BNZ3QX) for about $25 (AUD).

### Propellers

I was in the midst of designing my own props, when I realised that by the time I 3D print them and get the tolerances right, I could have some cheap ones already. The aerodynamic optimisation will have to wait a few design revisions, as this is primarily a control system design project.

Another consideration is whether to opt for 2- or 3-blade propellers. 2-blades offer more efficiency, 3-blades offer more lift. They also have lower structural requirements, due to the load being distributed over more blades. Triple blade it is.

### Motor

The drone brushless DC motor market is quite saturated, and it from my investigation, even more uncommon specifications are becoming easier to find. In terms of kV rating the general guideline is 1500-1700 for 7-inch drones, and higher for smaller drones. ECO MAX II 2807 is my primary candidate, but it will have to be tested.


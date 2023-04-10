---
layout: single
permalink: /projects/led_lamp/
title: "USB powered LED lamp"
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  overlay_image: /assets/images/projects_header.jpeg
author_profile: true
toc: true
toc_label: "Table of contents"
---


Small, USB powered LED lamp with up to 6 1W power LEDs. It uses diodes without a radiator, soldered directly onto the PCB. The power is delivered by the AP63203 step-down converter with up to 2A output current. The LEDs have forward voltage of about 3.1-3.2V at currents around 200mA,
that is why I decided to use a simple and cheap 3.3V converter with 1Ohm resistors splitting the power to every LED connected in parallel. This way I could also not solder in all of the LEDs, in the end I went with only 3 of them, as I thought it was enough for my usage.


# Schematic
The schematic and PCB were both designed using Altium Designer. Plase don't mind the LED pin 3 to GND conenction. It turned out that my LEDs actually don't have the center pin connected to anything, that is why I could do that to better manage the heat.
It might be different for your LEDs though, so please check that.

![Schematic](/assets/images/led_lamp/schematic.PNG)

# PCB design
The PCB is a single layer design, because I wanted to make it at home. I used an FR-4 board and etched it using B327 after doing the thermal transfer. 

![PCB](/assets/images/led_lamp/pcb.PNG)


![3d view](/assets/images/led_lamp/3dview.PNG)

# 3d CASE
The 3d model for the case was designed with Autodesk Fusion 360. It consists of the bottom case and top cover with empty space for a plexi panel. They are fastened together using M3 screws.
![case](/assets/images/led_lamp/case.PNG)


# Author
Krzysztof Sikora

Cracow, 04.2023
---
layout: single
permalink: /projects/nixie_power_supply/
title: "Nixie power supply"
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  overlay_image: /assets/images/projects_header.jpeg
author_profile: true
toc: true
toc_label: "Table of contents"
---


This power supply was designed for my friend, who needed a cheap high voltage PSU for his nixie tube clock.

# Nixie PSU
Input voltage is in the range of 9V to about 20V but I used a 12V power supply. The output is adjustable from 140V to over 200V,
with the maximum continous current about 20mA, which depends on the exact parts used (I used a different MOSFET and diode that I already had).

## Schematic
The schematic and PCB were both designed using KiCAD 6.0
![Schematic kicad](/assets/images/nixie_power_supply/schematic.PNG)

## PCB design
![PCB kicad](/assets/images/nixie_power_supply/pcb.PNG)


![3d view](/assets/images/nixie_power_supply/3dview.PNG)

## Parts used
* 220uF 16V electrolityc capacitor
* 300mOhm shunt resistor
* 1nF ceramic capacitor
* 330uH inductor
* 1kOhm, 470kOhm resistors
* generic fast switching diode and PNP transitor (1N914,BC557 on the schematic)
* IRF740 - power mosfet (you can try different ones to see which works best for you)
* 1N4004 diode
* 5k potentiometer
* 1uF capacitor for feedback filtering
* 4.7uF 400V output capacitor
* MC34063A dc/dc converter ic
* 2x connector

# Author
Krzysztof Sikora

Cracow, 02.2023
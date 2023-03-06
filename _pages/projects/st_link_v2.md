---
layout: single
permalink: /projects/st_link_v2/
title: "diy ST-LINK"
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  overlay_image: /assets/images/projects_header.jpeg
author_profile: true
toc: true
toc_label: "Table of contents"
---


ST-LINK is a programmer used with STM32 microcontrollers. It is sold by STMicroelectronics and by many other manufacturers and is included in a number of Nucleo/Discovery/etc. development boards.
Because of that, the schematics for it are available on the internet and you can build one yourself... and that is what I did.

# ST-LINK
My schematic was inspired by two diy projects, available under the following links: [STM32World](https://stm32world.com/wiki/DIY_STM32_Programmer_(ST-Link/V2-1)), [EmbdedBlog](https://embedblog.eu/?p=780). 
The design was then compared with one of STMs own designs from a Nucleo board.
You may think that the schematics could be easily reverse engineered, but you can't get the firmware for it, as it is proprietary STM softwa, right? Well, it seems someone has already done the job for us: [bootloader](https://github.com/Krakenw/Stlink-Bootloaders).


## Schematic
The schematic and PCB were both designed using KiCAD 6.0
![Schematic kicad](/assets/images/st_link/schematic.png)

## PCB design
![PCB kicad](/assets/images/st_link/pcb.png)


![3d view](/assets/images/st_link/3dview.png)

## Parts used
* STM32F103C8T6 microcontroller (you can use the CBT6 for more memory)
* TC1263 3.3V linear regulator
* IDC connector
* pin header for programming
* USB B connector
* 2x 0805 SMD LED
* 2x 220Ohm resistor
* 2x 100Ohm resistor
* 1MOhm resistor
* 3x 10kOhm resistor
* 2x 100kOhm resistor
* 2x 4.7kOhm resistor
* 1.5kOhm resistor
* 36kOhm resistor
* 470pF ceramic capacitor
* 1uF electrolytic capacitor
* 4x 100nF ceramic capacitor
* 2x 20pF ceramic capacitor



# Author
Krzysztof Sikora

Cracow, 03.2023
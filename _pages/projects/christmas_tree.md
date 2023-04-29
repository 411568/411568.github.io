---
layout: single
permalink: /projects/christmas_tree/
title: "PCB christmas tree"
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  overlay_image: /assets/images/projects_header.jpeg
author_profile: true
toc: true
toc_label: "Table of contents"
---


This project is a tiny pcb christmas tree with blinking leds. I found them on aliexpress ([LEDS](https://pl.aliexpress.com/item/32899224291.html?spm=2114.search0104.3.173.4e783c3abS4jLt&ws_ab_test=searchweb0_0%2Csearchweb201602_2_10065_10068_319_10892_317_10696_453_10084_454_10083_10618_10304_10307_10820_10821_538_537_10302_536_10843_10059_10884_10887_100031_321_322_10103%2Csearchweb201603_51%2CppcSwitch_0&algo_expid=81e95498-2155-4ab7-ab13-5b16242550b5-25&algo_pvid=81e95498-2155-4ab7-ab13-5b16242550b5&gatewayAdapt=glo2pol)).
They only require connecting to power supply and with a single battery you might even get away without using the resistors. Still, I decided to use 220Ohm resistors for the red, yellow and orange leds with 100Ohm for the blue ones. 
I hope that you will be able to buy those and maybe some other designs before chrismas this year at tindie.com.

# Schematic
The schematic and PCB were both designed using Altium Designer and manufactured at JLCPCB. The PCB is panelized so that 4 of them take up almost the whole 100x100mm board space. 
Because of that I only paid $2 for 20 of them.

![Schematic](/assets/images/christmas_tree/schematic.PNG)


# PCB design
![PCB](/assets/images/christmas_tree/pcb.PNG)

![3d view](/assets/images/christmas_tree/3dview.PNG)

![build](/assets/images/christmas_tree/tree.jpg)


# Parts list
* LEDs - as in the description
* battery mount - BR1220 (Keystone 3001)
* switch - PCM12SMTR
* resistors - 220Ohm/100Ohm 0603


# Project files
You can find the altium designer files under the [link](https://github.com/411568/Christmas_tree_PCB).


# Author
Krzysztof Sikora

Cracow, 04.2023
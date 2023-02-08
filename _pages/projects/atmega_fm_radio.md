---
layout: single
permalink: /projects/atmega_fm_radio/
title: "Atmega8 FM radio"
header:
  overlay_color: "#5e616c"
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  overlay_image: /assets/images/projects_header.jpeg
author_profile: true
toc: true
toc_label: "Table of contents"
---


This project is a revision of one of my old designs, created a long long time ago when atmel atmega chips where still dirty cheap.

You can find all the project files on my github: [github project](https://github.com/411568/Atmega8_FM_radio)

It contains two seperate boards: 
 - main_radio_board - this one contains an Atmega8 microcontroller, TEA5767 FM radio module, PAM8302 amplifier module and power connector. 
 - display_and_controls_board - this one is specificly designed to fit in an old Unitra radio case, it has LEDs used as radio frequency indicators, rotary encoder for changing the frequency, potentiometer for volume and some additional buttons.


# Radio board
My FM radio is based on the TEA7567 module, that is connected to an Atmega8A-PU microconotroller via I2C. Then it's output goes to the connector, then on the main panel passes through a logarithmic potentiometer for volume control 
and comes back to the PAM8302 D-class amplifier module. I chose it because it works well with my speaker, which is the one used in the original Unitra radio (it is probably over 40 years old and still works very well).


## Schematic
The schematic and PCB were both designed using KiCAD 6.0
![schematic kicad](/assets/images/atmega_fm_radio/schematic_1.png)

## PCB design
![PCB kicad](/assets/images/atmega_fm_radio/pcb_image_1.png)
![3d view](/assets/images/atmega_fm_radio/pcb_image_2.png)


## Connector pins
![pcb view with pinout](/assets/images/atmega_fm_radio/pcb_pinout.png)

In the image above you can see the 9V DC input jack location, the speaker output connector and two pin headers (IDC connectors).

J4 connector pinout (all of these are generic GPIO pins of the Atmega8):
- 1  - switch 3
- 2  - switch 1
- 3  - NC
- 4  - LE(ED1)
- 5  - SDI
- 6  - switch 4
- 7  - switch 2
- 8  - switch 0
- 9  - OE(ED2)
- 10 - CLK

J3 connector pinout:
- 1  - TEA5767 output (to potentiometer)
- 2  - transistor 0
- 3  - transistor 2
- 4  - encoder B
- 5  - 5V DC
- 6  - 9V DC
- 7  - PAM8302 input (from potentiometer)
- 8  - GND
- 9  - transistor 1
- 10 - encoder A


## Atmega8 code


## Parts used
As it was just a revision of an older schematic, I did not bother to try and redesign it with newer uC etc. I just used the parts from the previous version (soldered onto a prototype board) or those I had lying around. 
Because of that the design may look a bit peculiar and I decided not to make a BOM file for it. Let me just list them in here for you:
* Atmega8A-PU microcontroller
* TEA5767 module
* PAM8302 amplifier module
* 2x IDC connector for the front panel
* LM317 for power step-down
* 9V DC jack input
* 3x ceramic 100nF capacitor
* 10uF and 4.7uF electrolytic capacitors
* 3x 10k resistor


# Front panel board


## Schematic

## PCB design

## Parts used


# Assembled project



# Author
Krzysztof Sikora
Cracow, 01.2023
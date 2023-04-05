---
title:  "DC/DC converters testing"
search: true
categories: 
  - Jekyll
last_modified_at: 2023-04-051T08:06:00-05:00
---


Below you can see the tables and plots from my tests of 3 dc/dc converters: 
* MP8862
* MP28167
* AP63203

I wanted to compare the two MP... converters and see which one will be better to implement it in my power supply design. 

On the other hand, AP63203 is a step-down converter for 3.3V 2A output current, that requires as little as 1 inductor and 4 capacitors to work correctly.
That is why I needed to try it out when I saw it and based on the results of my tests, I can recommend it for any design requiring low voltage supply
for microcontrollers etc, when the LDO would be wasting too much power and you still want to keep the cost and size to the minimum.


## Test equipment
For my tests I used a lab power supply, with 10mA current resolution and a constant current load with 1mA, 10mV accuracy. 


# AD63203 test


# Test board files
You can find the KiCAD files for the test board on my github:
[github link](https://github.com/411568/MP28167-MP8862_test_board)

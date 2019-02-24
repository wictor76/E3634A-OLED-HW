# HP/Agilent E3634A OLED display to replace old VFD

Big thanks to qu1ck!
See [Original design](https://github.com/openscopeproject/HP34401a-OLED-HW) for more information.

Original HP 34401A design was made for different OLED display. This is modified for different display pinout 
and to have USB connector pointing downwards, since I don't want to make hole to front panel display. 
Input power is also taken from front panel voltage regulator.
This board could be used also in 34401A and other PSUs using similar front panel design. 

This board was designed in KiCad 5 and uses exclusively standard KiCad libraries.

# Schematic

![schematic](https://github.com/wictor76/E3634A-OLED-HW/raw/master/image/schematic.png)

# Board

![board_front](https://github.com/wictor76/E3634A-OLED-HW/raw/master/image/front.png)
![board_back](https://github.com/wictor76/E3634A-OLED-HW/raw/master/image/back.png)

# BOM

[Interactive BOM](https://htmlpreview.github.io/?https://github.com/wictor76/E3634A-OLED-HW/master/bom/ibom.html)

# OLED

OLED display needs to be configured for parallel data access. This display was initially configured
 for 4 wire SPI, so R18 resistor was moved to R17 to enable parallel 80XX mode.

See following image to locate resistors:
![oled](https://github.com/wictor76/E3634A-OLED-HW/raw/master/image/oled.jpg)

# ESP8266 WiFi RGBWW LED Dimmer v1.2
Custom Hardware board for controlling 5 Led Channels via PWM (RGB + Warm/Cold White). It is designed for max current ~4.5A per Channel.

# Changelog

* 1.2 (16.02.2016)
  * improved the layout for better EMV
  * added buffer capacitor for dc converter
  * added filter capacitor close to ESP8266
  
* 1.1 (01.02.2016)
  * connected ADC 
  * some layout improvements

# Parts
- 1x ESP8266, ESP-12 format
- 1x XM1584 Power converter (set to 3.3v!)
- 5x IRLZ44N Mosfet (logic level gate threshold)
- 10x 10k resistors, 0805 (R1 - R6, GPIO2, GPIO15, REST, CH_PD)
- 1x 1k resistors, 0805 (R7)
- 1x 1000 µF Elko RM 3.5 mm (C1) 
- 1x 100 µF Elko RM 2.5 mm (C3)
- 1x 100 nF capacitor 0805(C3)
- 3x 5,08mm 2pin terminal block
- 1x 5,08mm 3pin terminal block
- 1x 2,54mm 4pin header
- 1x Micro SMD Tact Switch 2 pin 3*6*2.5 mm 


# Assembly
Assembly of the PCB Board is straight forward, solder all parts to the PCB.

__Caution :__ before soldering the esp module to the PCB, set the output voltage of XM1584 converter  to 3.3v

### Recommended steps
- Start with soldering the smd resistors
- __Ensure the output voltage of XM1584 converter is 3.3v before continuing__. 
- Solder the XM1584 Power Board 
- Solder ESP8266 Module 
- Optional: solder SMD Tact Switch
- Solder Elkos
- Solder Terminal Blocks, 4pin header 
- Solder FETs


# Firmware
Firmware is still work in progress.

Latest can be found here:
https://github.com/patrickjahns/esp_rgbww_controller_fw

# Modifying
The schematic and board files are compatible with eagle 7.2+

## Ideas
Here are some ideas for future revisions
- ~~connect ADC to detect power failure~~ 


# Resources

* [ESP RGB Project](https://github.com/RiRomain/esp-dimmer-hardware)
* [H801 Wifi Controller Hack](http://chaozlabs.blogspot.de/2015/08/esp8266-in-wild-wifi-led-controller-hack.html)


# Credits
Thanks to RiRomain for his excellent documentated [ESP RGB Project](https://github.com/RiRomain/esp-dimmer-hardware)



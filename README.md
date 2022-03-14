# Eclipse KUKSA CANOPi  Hardware 

This repository contains information and manufacturing files for the CANOPi automotive prototyping plattform.


<img src="./hw_doc/img/CANOPi_bottom_frei.png" height="200"  style="margin:10px 10px">
<img src="./hw_doc/img/CANOPi_top_frei.png" width="200"  style="margin:10px 10px">

The Eclipse KUKSA CANOPi is a baseboard for the [Raspberry Compute Module 4 (CM4)](https://www.raspberrypi.com/products/compute-module-4).

With the CANOPi you have all the ingredients for hacking vehicles and prototyping Software Defined Vehicle functions and applications.

 * Compatible with the Raspberry Pi ecosystem thanks to the CM4
 * Up to 8GB of RAM and up to 32GB eMMC or any size micro SD card storage
 * integrated SIM card slot and M2 slot to add cellular connectivity
 * Can be powered via a vehicle's [OBD Port](https://en.wikipedia.org/wiki/On-board_diagnostics#OBD-II) 
 * [STN2120 OBD-II](https://www.obdsol.com/solutions/chips/stn2120/) to access vehicle data on OBD (only CAN supported by hardware)
 * Two [MCP251xFD](https://www.microchip.com/en-us/product/MCP2518FD) based [CAN-FD](https://en.wikipedia.org/wiki/CAN_FD) interfaces allowing interfacing two vehicle classic CAN or CAN FD busses directly.
 * [PCF85036A Realtime clock](https://www.nxp.com/products/peripherals-and-logic/signal-chain/real-time-clocks/rtcs-with-ic-bus/tiny-real-time-clock-calendar-with-alarm-function-and-ic-bus:PCF85063A)


## What you can find here
 * Find schematics board renders and BOM lists in [./hw_doc/](./hw_doc/)
 * You can find GERBER files needed to manufacture the PCB in [./manufacturing](./manufacturing) 
 * [Altium Designer](https://www.altium.com/altium-designer) EDA project file nn case you want to modify the schematics can be found in [./EDA](./EDA). 

## How to setup

If you set up a fresh CM4 that has never been used before in CANOPi you need to update the EEPROM first

 * [Updating CM4 EEPROM for CANOPi](./sw_doc/update_eeprom.md)

 In order to make full use of all hardware components, you need to configure your Raspberry OS

  * [Enabling Hardware support in your OS](./sw_doc/configure_raspberryos.md)
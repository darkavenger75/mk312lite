# mk-312 lite

## Introduction

A smaller, lighter, cheaper and easier to assemble version of the mk-312 with most of its functionality

- LiFePO4 instead of Pb battery
- 90 x 120 mm single PCB design
- Most components SMT on bottom side (JLCPCB can do most of the work)
- No inputs, though

## Board ordering instructions

PCB
- Default settings by JLCPCB work fine. Feel free to choose different color, etc. Lead-free recommended for the sake of the environment.

Assembly
- Economic, Bottom side, as many PCBs as you wish (minimum 2). "Confirm Parts Placement" recommended. 
- Automatic selection of parts after uploading BOM and CPL worked well, but better check for errors. 
- Check part placement and rotation, esp. ATmega, transistors and 5V DC/DC converter (K7805).  

## Parts ordering information

You will in addition require all pin-through-hole parts, see full BOM (eagle_cam_job_files/mk312lite_V2_full_BOM.csv). Most parts you can order from Mouser. Do not forget the buttom covers and knobs for the potentiometers. 
In addition, you will have to order
- 2 pcs. PJ-301C XKB 1/8" phone connectors (e.g. eBay)
- A 12V 2Ah LiFePo4 4-cell battery with BMS and connector matching the one you used on the board. I got mine from Eremit in Germany. You can use a 3-cell LiPo battery pack instead (there is a LDO voltage regulator on the 9V rail), but the R5/R6 voltage divider must be adjusted to avoid incorrect low battery warning/shutdown.
- A matching external CHARGER for your battery pack with 5.5/2.1 mm connector, center positive. Do NOT just connect a power supply without current limiter.   

## Board assembly Instructions

- The two transformers, battery connector and polyfuse go to the bottom of the PCB (or the front panel will not fit).
- Nothing special regarding the assembly of the top side.
- Ensure polarity of your battery pack and charger is correct, or things may get fried. 

## Firmware

The firmware has not been modified, for instructions see the "firmware" folder. 

## Case

Front panel still in design. Will go directly on top of the PCB, the battery pack below. Bottom closed with plain aluminum panel.  
You will also require some simple 3D printed (or milled) plastic profiles to hold everything together. Details coming!

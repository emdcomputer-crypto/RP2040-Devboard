# RP2040 Devboard

This is my custom RP2040 devboard for Hack Club Half Life week 5. I followed the guided devboard project and made my schematic and PCB in KiCad. The board has USB-C, an RP2040, flash memory, a 12 MHz crystal, an LDO and headers to get to the GPIO pins.

![JLCPCB part selection for the board](Pictures/1.png)

![The KiCad schematic](Pictures/11.png)

![The routed PCB in KiCad](Pictures/31.png)

## How it works

The RP2040 is the main chip on the board. It uses external flash memory to store the program and a 12 MHz crystal for its clock. USB-C brings power and the USB data connections onto the board. The LDO regulates the power for the 3.3V parts, and the headers bring the GPIO pins out so they can be used for other things.

## How I made it

i started by following the guide and building the schematic in KiCad. There was a lot of wiring to do for the USB-C, flash memory, crystal and all the GPIO headers. I also had to check the RP2040 datasheet and make sure the parts and footprints were right.

The PCB was the hardest part for me because there wasnt much space and the traces kept getting in the way of each other. I moved things around a lot and added vias to get the connections onto both layers. After routing I worked through the DRC errors one by one, cleaned up the silkscreen and exported the files for JLCPCB.

## Bill of materials

The full parts list is in [BOM.csv](BOM.csv). My JLCPCB estimate was:

| Item | Cost |
| --- | ---: |
| Production and assembly | $58.28 |
| Estimated shipping and tax | $55.89 |
| Total | $114.17 |

This was $14.17 over the $100 Tier 3 funding amount.

## Project files

- [Hardware](Hardware/) - KiCad schematic, PCB layout and project files
- [FabricationFiles](FabricationFiles/) - files exported for PCB manufacturing
- [BOM.csv](BOM.csv) - project cost and parts list
- [JOURNAL.md](JOURNAL.md) - my work notes while making the board

## Guide

I followed the [Hack Club Blueprint RP2040 Devboard guide](https://blueprint.hackclub.com/starter-projects/devboard).

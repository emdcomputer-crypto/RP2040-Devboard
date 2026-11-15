# RP2040 Devboard

This is my custom RP2040 devboard for Hack Club Half Life week 5. I followed the guided devboard project and made my schematic and PCB in KiCad. The board has USB-C, an RP2040, flash memory, a 12 MHz crystal, an LDO and headers to get to the GPIO pins.

<img width="1916" height="929" alt="1" src="https://github.com/user-attachments/assets/b21a2a65-0c6e-4e79-b7ff-fa998fd5c0fd" />


<img width="1205" height="856" alt="11" src="https://github.com/user-attachments/assets/b4fd1351-585d-419d-bcc5-202c9e839537" />


<img width="1919" height="1025" alt="31" src="https://github.com/user-attachments/assets/f7667b95-8ae9-4330-85b6-8989ad95e70d" />


## How it works

The RP2040 is the main chip on the board. It uses external flash memory to store the program and a 12 MHz crystal for its clock. USB-C brings power and the USB data connections onto the board. The LDO regulates the power for the 3.3V parts, and the headers bring the GPIO pins out so they can be used for other things.

## How I made it

i started by following the guide and building the schematic in KiCad. There was a lot of wiring to do for the USB-C, flash memory, crystal and all the GPIO headers. I also had to check the RP2040 datasheet and make sure the parts and footprints were right.

The PCB was the hardest part for me because there wasnt much space and the traces kept getting in the way of each other. I moved things around a lot and added vias to get the connections onto both layers. After routing I worked through the DRC errors one by one, cleaned up the silkscreen and exported the files for JLCPCB.

## Bill of materials

The full parts list is in the picture above but you don't need to copy it as i placed all of them in the BOM file for jlcpcb. My JLCPCB estimate was:

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

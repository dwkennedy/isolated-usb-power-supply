# isolated-usb-power-supply

BOM

Quanity, Description, Part Number
- 1, Recom RP15-1205SA  9-18V to 5V dc/dc isolated power supply, P/N 919-RP15-1205SA Mouser
- 2, SMD MLCC CAPACITOR CER 10UF 25V size 1812, P/N 445-7908-1-ND DigiKey
- 2, SMD MLCC CAPACITOR CER 470PF 2KV size 1808, P/N 445-11906-1-ND DigiKey
- 1, SMD FUSE BOARD MOUNT 1.6A 32VDC size 0603, P/N SF-0603SP160-2CT-ND DigiKey
- 1, SMD CMC 160UH 2.3A 2LN (common mode choke), P/N 283-4436-1-ND DigiKey
- 2, CONN PCB USB RA FEM TYPE A SMD, P/N AE11187-ND DigiKey
- 2, powerpole right angle contact horizontal (bottom) P/N 1336G1
- 1, powerpole PP15/45 housing, black P/N 1327
- 1, powerpole PP15/45 housing, red P/N 1327
- 4, #3 pan head screws, 5/8" long

FILES

- usb_power.brd    EAGLE board layout
- usb_power.sch    EAGLE schematic
- enclosure.SLDPRT Solidworks part, enclosure body
- enclosure.STL    enclosure rendered in STL for printing
- cover.SLDPRT     cover of enclosure
- cover.STL        cover rendered in STL for printing

Requires Doug's EAGLE library https://github.com/dwkennedy/eagle-library

TODO

Notes from first spin of PCB: pads for SMD fuse are too widely spaced for 0603 part.  SMD fuse should be changed to another part, because 0603 is difficult to hand solder. Also, holes and pads for RECOM RP-15-1205SA are too small after plating.  The USB part footprint doesn't have exposed copper to solder the tabs that go through the board. Hot glue fixes the wobbly USB connectors :)  Might consider moving USB connectors a little farther from the RP15-1205SA can in case they need to be resoldered at some point.

Improvements: add biasing resistors to 5VDC output to enable higher current on devices that support that charging protocol.  Identify a isolated DC/DC module that is less expensive and/or higher current than the RP15-1205SA.

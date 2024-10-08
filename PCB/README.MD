# TOTEM-SHIFT PCB FILES

I have modified the original PCB extensively, so here is a list of the largest changes:
- Moved the middle finger column down by approx 2.3mm, as it felt a little high compared to other boards.
- Made the underside of the XIAO easier to solder through a larger cutout.
- Moved the battery contact points above the diodes for the larger size battery cavity.
- Moved the diodes to the rear to make a little more space for the battery and for a clean top PCB.
- Rerouted many traces, cleaned up others and added many diagonal angles for aesthetic purposes and to remove acute angles which are more prone to manufacturing errors.
- Removed the TRRS connector completely as this is a wireless-centric design now.
- Replaced the reset and power switches with hidden ones inside of the top plate, where the TRRS used to be. This gives the case a completely clean look.
- Removed the large color silkscreens as while they were super nice, it was not possible for me to edit them in a way that looked good since I don't have the source files.
- Moved a few other things to make place for these changes.
- Tried to realign one of the holes on the right as it wasn't mirrored properly.
- Everything has been updatd for KiCad 8.0 and gerber files should be able to be easily uploaded to PCB manufacturer websites, I've provided my gerber zip file prepared by JLCPCB's plugin.

> **Note**
> As a reminder: The PCB is modified enought that this version will not be compatible with existing PCBs or cases for the original TOTEM.

![TOTEM PCB](/PCB/TOTEM-SHIFT%200.4%20PCB.jpg)

# TOTEM-SHIFT FUTURE

What I'm thinking of working on next after this build is complete and I'm satisfied using it.

- [ ] Utilize additional pins from NFC/Sense for ?
- [ ] Implement support for LCD on the board or on the dongle (for layer visibility and style)
- [ ] Implement support for encoder
- [ ] Implement support for pointing device (touchpad, trackpad, mini trackball)
- [ ] Recreate a similar board from scratch that's fully reversible


# TOTEM PCB FILES

## MANUFACTURING
If you want to get the PCB made you need to download the [ZIP](/PCB/totem_0-3/totem_0-3_gerbers.zip/) and upload it to the website of the manufacture 
I can recommend [JLCPCB](https://jlcpcb.com/), [Seeed Fusion](https://www.seeedstudio.com/fusion_pcb.html) or [PCBway](https://www.pcbway.com/).

- Download [the ZIP file](/PCB/TOTEM-SHIFT%200.4/production/TOTEM-SHIFT_split_keyboard_0.4.zip)
- Upload the ZIP file to the website of the manufacturer.
- Sometimes the Gerber preview from JLCPCB can't display the PCB, even when the files are fine. In this case use these dimensions: 258.7mm * 94.35mm.
- PCB Thickness: 1.6mm
- Layers: 2
- Different designs: 2 (because both halves are not the same).
- PCB Qty as much as you like, but minimum is always 5. One PCB is a full keyboard.
- PCB Color Black (or any other color you like).
- No impedance control.
- Surface Finish HASL (with lead) if you want the easiest soldering experience or LeadFree HASL.
- Remove Order Number: Yes

![TOTEM PCB](/docs/images/TOTEM_pcb.png)

***

## CHECK PINOUT OR TRACES

If you only want to check the traces or see what is connected to which pin you can take a look at these graphics.
You can also take a look at the [schematics](TOTEM_0-3_schematics.pdf) and the [PCB](TOTEM_0-3_PCB.pdf) as PDF.

![TOTEM pinout](/docs/images/TOTEM_pinout.png)

***

![TOTEM traces](/docs/images/TOTEM_traces.svg)

***

## TAKE A DEEPER LOOK OR MODIFY 

You can download the project if you need to take a deeper look or modify something. You need the Open Source software [KiCad](https://www.kicad.org/) to open it.

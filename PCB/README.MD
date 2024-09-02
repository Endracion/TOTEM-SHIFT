# TOTEM-SHIFT PCB FILES

I have modified the original PCB extensively, so here is a list of changes:
- Moved the middle finger column down by approx 2.3mm, as it felt a little high compared to other boards.
- Made the underside of the XIAO easier to solder through a larger cutout.
- Moved the battery contact points above the diodes for the larger size battery cavity.
- Moved the diodes to the rear to make a little more space for the battery.
- Rerouted many traces, cleaned up some others and added many diagonal angles for aesthetic purposes and to remove acute angles on traces.
- Removed the TRRS connector completely as this is a wireless-centric design.
- Replaced the reset switch with a very common Omron style 6x6 tactile switch, which sits where the TRRS used to be (mostly because I have a ton of them and they're very solid).
- Removed the large color silkscreens as while they were super nice, it was not possible for me to edit them in a way that looked good since I don't have the original files.
- Moved a few other things to make place for these changes.
- Tried to realign one of the holes on the right as it wasn't mirrored properly.
- Everything has been updatd for KiCad 8.0 and gerber files should be able to be easily uploaded to PCB manufacturer websites now (old ones were giving me errors).

> **Note**
> As a reminder: The PCB is modified enought that this version will not be compatible with existing PCBs or cases for the original TOTEM.

# TOTEM PCB FILES

## MANUFACTURING
If you want to get the PCB made you need to download the [ZIP](/PCB/totem_0-3/totem_0-3_gerbers.zip/) and upload it to the website of the manufacture 
I can recommend [JLCPCB](https://jlcpcb.com/), [Seeed Fusion](https://www.seeedstudio.com/fusion_pcb.html) or [PCBway](https://www.pcbway.com/).
If you want the silkscreen in yellow [AllPCB](https://www.allpcb.com/online_pcb_quote_new.html) is a pretty affordable choice.

- download [the ZIP file](/PCB/totem_0-3/totem_0-3_gerbers.zip/)
- upload the ZIP file to the website of the manufacturer.
- sometimes the Gerber preview from JLCPCB can't display the PCB, even when the files are fine. In this case use these dimensions: 258.7mm * 94.35mm
- PCB Thickness 1.6mm
- 2 layers
- PCB Qty as much as you like. One PCB is a full keyboard.
- PCB Color Black (or any other color you like)
- No impedance control
- Surface Finish HASL(with lead) if you want the easiest soldering experience or LeadFree HASL.
- Remove Order Number Yes

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

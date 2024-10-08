# TOTEM BUILD GUIDE

> **Warning**
> The updated build guide is still missing a few pictures.

## PART LIST

### REQUIRED PARTS

| Part name       | Count | Remarks | 
| :-------------- | :---: | :------ |
| TOTEM PCB       | 01 | You can find the files for it [here](/PCB//TOTEM-SHIFT%200.4) |
| Seeed XIAO BLE  | 02 | Uses nRF52840 chipset. The best place to get them is direct from SEEED; suggesting the [3 pack wtih free shipping](https://www.seeedstudio.com/Seeed-Studio-XIAO-nRF52840-3PCS-p-5921.html). |
| Choc key switch | 38 | Kailh Choc low profile key switches |
| diodes 1N4148W  | 38 | These are surface mount diodes in SOD123 package |
| 1u Choc keycaps | 38 | GEIST recommends MBK, LDSA or CFX keycaps, but I used the [MOTE](https://www.printables.com/model/864126-mote-choc-low-profile-flat-keycaps/remixes) and the [15 degree remix](https://www.printables.com/model/1000549-mote-remixed-choc-low-profile-flat-keycaps-with-mo) for a keywell feeling |
| reset button    | 02 | 3x6x4.3mm DIP 2 pin tacticle switches |
| power switch    | 02 | MSK-12C02 |
| Lipo battery    | 02 | There is space for a battery of 7x15x42mm with capacities up to ~180 mAh; I used 401230 |
| USB-C cable     | 01 | For charging the keyboard or connecting it to your PC |


### OPTIONAL PARTS

| Part name              | Count | Remarks | 
| :--------------------- | :---: | :------ |
| switch socket          | 38 | Switch sockets for Kailh low-profile choc switches |


### 3DP CASE PARTS

| Part name              | Count | Remarks | 
| :--------------------- | :---: | :------ |
| 3D printed case        | 02 | Find the case files [here](https://www.printables.com/model/1033457-totem-shift-wireless-ble-redux-split-splay-keyboare) |
| 4mm M2 hex head screws | 08 | The hex head is important, and the material needs to be ferrous so that the magnets can attach to them. |
| 4x2mm round magnets    | 08 | These will align with the round screws to magnetically atttach the top plate |
| rubber feet            | 08 | Any size you prefer |


## INTRODUCTION

Here is an overview of where and on which side each component needs to be soldered (click on the image to see a larger version).

![TOTEM solder guide](/docs/images/TOTEM_solderguide.png)


***

## BREAK OFF HALVES

The PCB comes in one piece. You need to break it into two halves.

![TOTEM PCB](/docs/images/buildguide/pcb_top.jpg)

After breaking them apart, you're left with some sprue marks, which you can remove with a file if you like, but you don't need to.

> **Warning**
> You should wear a mask in a well ventilated area while doing this since the FR4 dust is extremely toxic.

![PCB sprue marks](/docs/images/buildguide/side_01.jpg)

I paint the edges black using a sharpie, so they fit better with the top and bottom, but that's optional too.

![PCB edges](/docs/images/buildguide/side_02.jpg)


***

## DIODES

The diodes need to be soldered on the top of the PCB. Pay attention to their orientation:  They have a small line on one side, which should be on the side the arrow on the PCB is facing to.

<p align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/buildguide/diodes_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/buildguide/diodes_bright.svg">
  <img alt="diode orientation" src="/docs/images/buildguide/diodes_dark.svg">
</picture>
</p>

Apply a small amount of solder on one pad.

![Solder on one pad](/docs/images/buildguide/diode_01.jpg)


Then use tweezers to place the diode on the pads and reheat the solder to secure the diode.

![Solder diode](/docs/images/buildguide/diode_02.jpg)


Now you can solder the second pad.

***
 
## SWITCH SOCKETS (optional)

Here you can apply the same technique as used for the diodes: Apply some solder on one of the pads first.

![switch sockets pad](/docs/images/buildguide/hotswap_01.jpg)

Then place the switch socket in the silk screen markings. The orientation matters here too. Especially if you plan on using the case.

<p align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/buildguide/socket_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/buildguide/socket_bright.svg">
  <img alt="hotswap socket orientation" src="/docs/images/buildguide/socket_dark.svg">
</picture>
</p>


![hotswap socket right and wrong orientation](/docs/images/buildguide/hotswap_02.jpg)


Then reheat the solder. 
Apply some pressure with a pair of tweezers to make sure the socket is fully seated.\
Now solder the second pad.

![switch socket soldered](/docs/images/buildguide/hotswap_03.jpg)

***

## POWER SWITCHES

Apply a tiny bit of solder on the bigger, outer pads on top of the PCB. 

![power switch pads](/docs/images/buildguide/power_01.jpg)

The power switch has some tiny knobs on its bottom, which fit into the PCB holes. Hold it in place with tweezers and then reheat the solder on the pad. After this, you can solder the other pad and the three pins.

![power switch](/docs/images/buildguide/power_02.jpg)


***

## RESET SWITCHES

Insert the switch into the top of the PCB; aligne it so that it sits straight. Due to the leg shape, it should hold by itself, so you can then solder one leg at a time from the top.

I then turn the board over and use flush cutters to cut part of the producting legs off and add a little more solder from this side.

![reset switch](/docs/images/buildguide/reset_01.jpg)


***

## MICROCONTROLLER

> **Warning**
> First flash the microcontroller to make sure it works, before soldering it in. Especially since you can't use sockets for easy removal.

Place the microcontroller in its place. I used the headers they came with, and removed the last pin. This way, the XIAO is perfectly aligned and I can solder the last 2 unconnected pins while making sure everything stays flate.

Afterwards, you can remove the headers and continue soldering each pad.

> **Note**
> Make sure it sits flat on the PCB. Otherwise, the case won't fit.

Apply some flux and try to hold the iron at an angle where you touch the pads of the microcontroller and the PCB while adding solder.

![soldering MCU](/docs/images/buildguide/MCU_01.jpg)

The pads on the back are a bit harder to solder, but I believe in you! I've made the cutout a lot larger than the original, so it should be a little easier. Apply the same technique as on the front: Try to touch the pads on the microcontroller and the PCB before adding solder. 

First off, if you didn't choose castellated half holes (which I'm too cheap for), you'll have extra pieces of copper in these half holes from the routing step, which you'll need to carefully wedge out and remove. Here I used a needle to push it away from the hole, then some fine tweezers to rock it side to side carefully, so that it detaches without ripping anything. This way you're left with a nice solderable surface.

![soldering MCU back](/docs/images/buildguide/MCU_02.jpg)


***

## BATTERY

> **Warning**
> Before attaching the battery in any way to the PCB set the power switch to off (right on both sides).

You can see which cable needs to go in which eye by the silkscreen below the eyes. Red is + / Black is -. Do make sure your manufacturer respected this. The red wire is usually isolated with tape or something similar when being shipped.

![battery face](/docs/images/buildguide/batt_face.jpg)

Attach the wires of the battery to the pads and solder them in.

![Ouch](/docs/images/buildguide/it_stings.jpg)


***

## CLEANING

You can use an old toothbrush, some cotton swabs and some isopropyl (closest to 99% is best) to clean it from flux residues. 


***

## FIRMWARE

If you have not already flashed the firmware to the microcontroller you should do it now.\
[Here](https://github.com/Endracion/zmk-config-totem-shift) you can find the ZMK firmware for the TOTEM.\

Probably a good idea to also install switches to make sure all of them work, before inserting the board into the case.

![PCB with switches](/docs/images/buildguide/pcb_switches.jpg)


***

## CASE

First, place the PCB on the bottom plate, making sure the integrated standoffs go through the holes and fits snugly.


Next, loosely screw in the midplate with the M2 screws straight into the bottom plate. At this step you'll want to push in a few switches so that they clip into the midplate and align it properly.


I placed 5 (corners and middle) for this purpose, and then finished tightening the screws (careful not to overtighten though, it just needs to be finger tight, don't snap the plastic).


My case doesn't have specific locations for the rubber feet if you're installing them, so choose where you'd like to place them.


Next we move on to the top case. The magnet holes are fitted with crush tabs, which allow for different printer tolerances. You will have to push in these magnets into the bottom with a bit of force. I like to place them on the tip of my pliers and push down. Note that there is a little indentation below that allows you to pry the magnet out if anything happens or it doesn't go in straight.

You may have to trim the sides of this little tab in the middle of the plate, but only very slightly at a time, and check for the fit, as you want it to be friction fit when you press down on it, but still allow for it to be removable.

***

## FINAL BUILD

This is what the final keyboard will probably look like. 

![final build](/docs/images/buildguide/final.jpg)



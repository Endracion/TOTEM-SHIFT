<picture align="center">
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_bright.svg">
  <img alt="TOTEM logo" src="/docs/images/TOTEM_logo_dark.svg">
</picture>

<h1 align="center">T O T E M - S H I F T</h1>

TOTEM-SHIFT is a modified 38 keys column-staggered split keyboard originally by GEIGEIGEIST.

This TOTEM-SHIFT version aims to allow for a larger battery and emphasize styling options through a swappable top plate held with magnets ([demo](https://www.youtube.com/watch?v=WX03MpgzbRs)). Meant to be used with a SEEED XIAO BLE (no longer supports the RP2040 with the TRRS port removed) for a wireless only build.

**WHY** a swappable top plate? Well I'm sure everyone has asked themselves at least once, which case should I go for? And then you're half locked into it.
I want to be able to change my mind, to change colors, logos, motifs or other surface effects to go with the style I want that day, so why not allow myself to do just that with a swappable top plate!

It was created for the SEEED XIAO keyboard contest by GEIGEIGEIST.\
[Here](https://www.hackster.io/geist/totem-a-tiny-splitkeyboard-with-splay-cb2e43) you can read about the process of making it.

Note that most of the guides and links will remain unchanged, the major changes will be to the 3D printed case design, as it uses the [TOTOEM Redux by VOID](https://www.printables.com/model/840146-totem-redux) case files as base, which are better suited to FDM 3D printing.

> **Note**
> The PCB is modified enought that this version will not be compatible with existing PCBs or cases for the original TOTEM.

***

## LAYOUT

![TOTEM layout](/docs/images/TOTEM_layout.svg)

***

## PCB

[Here](/PCB/TOTEM-SHIFT%200.4) you can find the KiCad files and Gerbers for the TOTEM.

Gerber files to upload for production are found [here](https://github.com/Endracion/TOTEM-SHIFT/tree/main/PCB/TOTEM-SHIFT%200.4/production).

***

## CASE

You can use the TOTEM without a case, but [here](https://www.printables.com/model/1033457-totem-shift-wireless-ble-redux-split-splay-keyboar) is the FDM 3D printed case I designed for it.

***

## BUILD GUIDE
  
The build guide for the TOTEM can be found [here](/docs/buildguide.md).

***

## FIRMWARE

[ZMK config](https://github.com/Endracion/zmk-config-totem-shift) for the TOTEM (wireless using the XIAO BLE)

The dongle version is coming at a later time.

***

## PHOTOS

This is the 3D printed TOTEM-SHIFT BLE Redux case with the MOTE keycaps.

This is the TOTEM in a black resin case

![TOTEM black resin](/docs/images/TOTEM_black_perspective.jpg)\
![TOTEM black resin](/docs/images/TOTEM_black_top.jpg)\
![TOTEM black resin](/docs/images/TOTEM_black_bottom.jpg)

***

## BUY 

If there is enough interest, I may do a production run for this modified version, please feel free to reach out.

***

## CREDITS

### ORIGINAL CREATOR

The amazing [GEIGEIGEIST](https://github.com/GEIGEIGEIST) whose design are beautiful and inspiring.
VOID who created a FDM optimized case [TOTOEM Redux](https://www.printables.com/model/840146-totem-redux).
eiga for the [MOTE keycaps]{https://www.printables.com/model/864126-mote-choc-low-profile-flat-keycaps}.

### INSPIRATION

The additional pinky key makes the TOTEM compatible with the layout boards like the [Balbuzard](https://github.com/brow/balbuzard) by [Tom Brow](https://github.com/brow) and the [Osprette](https://github.com/smores56/osprette) by [Sam Mohr](https://github.com/smores56) use, where you put the keybinding of the top left and right keys on an outer pinky key.

### HELP FIXING THINGS

People who helped GEIGEIGEIST create this board and fix stuff:

#### PCB
- [Marco "Bob"](https://github.com/GroooveBob)

#### CASE
- [Freya](https://github.com/freya-irl)
- [Bubbleology](https://github.com/bubbleology)

#### FIRMWARE
- [Cem Aksoylar](https://github.com/caksoylar)
- [Grinnie](https://github.com/regicidalplutophage)
- [Alaa Saad Mansour](https://github.com/AlaaSaadAbdo)
- [pekudzu](https://github.com/pekudzu)

If you build a TOTEM, GEIGEIGEIST would be pretty happy to see some pictures. And if you want to leave him a tip you can do so [here](https://ko-fi.com/geigeigeist) (but please don't feel pressured)


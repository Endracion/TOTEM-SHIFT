# TOTEM-SHIFT BLE REDUX CASE

These files can be found on Printables: [TOTEM-SHIFT Wireless BLE Redux Case](https://www.printables.com/model/1033457-totem-shift-wireless-ble-redux-split-splay-keyboar).
I've paired with the [MOTE](https://www.printables.com/model/864126-mote-choc-low-profile-flat-keycaps) keycaps and the [15 degree remix](https://www.printables.com/model/1000549-mote-remixed-choc-low-profile-flat-keycaps-with-mo) for more of a keywell feel.

I remixed the excellent [Totem Redux](https://www.printables.com/model/840146-totem-redux) by VOID and drew inspiration from BeeKeeb's rendition as well.
This case is made to be printed on an FDM printer, though it may work just fine on resin as well, I have not tested it.

My changes are as follows:
- Larger cavity above the diode area to accommodate a larger battery up to approx 7x15x42mm with capacities up to ~180 mAh.
- Removed all holes from the top cover in order to make it look cleaner and allow for future design choices (multi color motifs coming soon).
- Replaced these top screw holes with recessed magnet holes and crush tabs (so they're press fit) so that it can be magnetically attached and swapped ([demo](https://www.youtube.com/watch?v=WX03MpgzbRs)).
- Removed the countersink from the bottom plate so that the midplate is screwed into the bottom plate and acts as the magnet retention mechanism, along with the recessed feet holes as it won't print well on FDM.
- Removed the need for standoffs, everything screws or is pushed directly into the plastic for a tight fit.
- Removed all side holes except USB-C port since the TRRS port is removed and the reset and power switches are now hidden under the top cover.
- Adjusted many small parts of the assembly and redrew the bottom case to make FDM printing easier.
- Adjusted part heights to match 0.2 mm printing layer height and so that the midplate is the correct height to attach the switches to it and not create additional flexing.

![TOTEM-SHIFT BLE Redux case](/case/BLE%20Redux/TOTEM-SHIFT%20BLE%20Redux%20Case.jpg)

# ORIGINAL TOTEM CASE

Each half consists of a bottom and a top part (with an integrated switchplate) and is meant to be 3D printed in resin. 

I got good results from [JLCPCB](https://cart.jlcpcb.com/quote) (15€ + tax and shipping for a black or white version) and [PCBway](https://www.pcbway.com/rapid-prototyping/manufacture/?type=2&reffercode=TOP) (50€ + tax and shipping for a clear case).

Where possible use the STEP files, but the STL files should be fine too.

If you're sure you only will use the wired version you can also use the case without a power switch (USB) or use the case without a TRRS cutout if you plan on using the wireless version (BLE).

> **Note**
> The manufacturer will probably warn you about too thin sections, but it worked fine for me since these sections are pretty small.

![TOTEM case](/docs/images/TOTEM_case.png)
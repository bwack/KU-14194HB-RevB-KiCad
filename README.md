# KU-14194HB-RevB-KiCad

![3D render](3Dview_1.4-top.png?raw=true "Title")
![3D render](3Dview_1.4-bottom.png?raw=true "Title")

The rare KU14194HB C64 Motherboard schematics and layout. Retraced in and imported from SprintLayout.

Disclaimer: See DISCLAIMER.md

# Original bodges

This PCB is a replica. It includes the mistakes that Commodore made.

It is necessary to cut a trace above R37 on the bottom side, and add a 1K resistor from R37 and up to a via.
See the images folder to where to cut and add a resistor.

Piggyback a 100nF capacitor over CR1.

Notice how the main crystal oscillator Y1 body is grounded with a wire.

In later designs 250407 Reb B I think, 4 piggybacked diodes were introduced to protect the serial lines when hotplugging the disc drive.
I haven't added these myself, but I see the value of having those. I might add instructions here later on how to add the diodes.

# BOM

Please see the [BOM file](bom.csv).

# Interactive-BOM

[The interactive bom html page](https://htmlpreview.github.io/?https://raw.githubusercontent.com/bwack/KU-14194HB-RevB-KiCad/master/interactive-bom/ibom.html) is useful for assembling the board and finding signal traces by using a web browser. Try it here. For a BOM for ordering parts see the BOM above.

# Questions

* Feel free post questions in the issues section. I will provide more information here later.

# Change log

- 2020-01-23: V1.4 PCB improvements:
  - Expansion Port: Larger round solder pads for the shield. Same error in the original.
  - Expansion Port: Connector moved to center of shield. Some traces moved.
  - Left edge: Extended the PCB by 2.2mm.
  - Left edge: Increased track width of the power rails.
  - CAN shield: added two solder pads.
  - RF modulator: added solder pad.
  - Schematics: Rev 1.4. No change.
- 2019-11-12: V1.3 Fixes: Mostly missing values.
  - C88: "1000uF 25V" -> "470uF 50uF". Commodore said 1000 but used 470.
  - R31: "180" -> "1K". A mistake in the commodore schematics.
  - R52: "?" -> "330"
  - R53: "?" -> "100"
  - C86: "?" -> "82pF",
  - C36: "0.1" -> "20pF",
  - R22: missing trace. R22 = 0 Ohm. Parallel to C87 (NC). R22 doesn't matter.
  - C101: is a Y5U. VIC2's decoupling cap. Has a higher dielectric rating. Doesn't matter.
  - C70: 15pF 5%. This is a PAL only board. In later revisions, 16pF is used for NTSC.
 - 2019-11-10 V1.2 Added missing C14 10uF 25V electrolytic capacitor
- 2019-10-15 V1.1 Layout: Fixed missing keying-slot in user port.
- 2019-10-05 V1.0 First release.

# YouTube

A playlist of all the videos:

[![playlist](https://img.youtube.com/vi/iNxOm7G6efA/0.jpg)](
https://www.youtube.com/watch?v=iNxOm7G6efA&list=PLtQOf_JULmrTGLZCElGG_T1a01JSDP0CP)

# In the wind

forum64.de: The board has some threads at forum64.de (German). May require login.
* [KU-14194 Bestückungs-Thread](https://www.forum64.de/index.php?thread/96336-ku-14194-best%C3%BCckungs-thread/)
* [KU-14194](https://www.forum64.de/index.php?thread/95454-ku-14194/) (long group buy thread)
* [KU-14194 (Replika) ... wer schafft es als Erste/r? Aktuelle Sachstandsberichte ...](https://www.forum64.de/index.php?thread/95518-ku-14194-replika-wer-schafft-es-als-erste-r-aktuelle-sachstandsberichte/)

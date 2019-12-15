# KU-14194HB-RevB-KiCad

![3D render](Screenshot%20from%202019-10-06%2000-12-34.png?raw=true "Title")

The rare KU14194HB C64 Motherboard schematics and layout. Retraced in and imported from SprintLayout.

Disclaimer: Artwork not verified. Use at own risk.

# Change log

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
- 2010-10-05 V1.0 First release, not prototyped

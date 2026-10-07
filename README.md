# 3D Print Reference

### Description

The purpose of this repository is to document my personal process for
setting up and configuring a 3D printer. These configurations apply
specifically for 'bedslinger' styles of printers. Core-xy have fundamental
differences and some aspects of this document may not apply. The printer
I will be using for example is the Creality Ender 3 V2 Neo, which I have
had and used for years. For other printers, principles from this doc may
apply.

I've decided to begin this project to assist myself and other enthusiasts
with a straightforward, procedure for quickly setting up popular
Ender-style 'bedslingers'. Many modern printers enjoy enhancements that
automate or minimize these manual and often frustrating procedures. Also,
many references already exist for these platforms so I will attempt to not
reinvent the wheel in this process. As I am still a proud owner of one of
these machines, finicky as they might be, I will continue to support their
configuration, customization and freedom as long as possible. Long live
the Ender!

Thanks for checking out this repository, and Happy printing.

## Manual Adjustments
These steps apply to **bedslinger** printers; CoreXY printers require a
different process.

### Manually Set the Z Offset

Level the bed at each of its four corners:

1. Heat the bed. Heating the nozzle is optional. **Caution:** hot printer
   components can cause burns.
2. Manually set the Z height to `0`.
3. Move the nozzle to a corner of the bed (for example, `X190 Y190`).
4. Place a `0.102 mm` feeler gauge—approximately the thickness of standard
   printer paper—between the nozzle and bed.
5. Adjust that corner with the bed-adjustment dial, rather than the printer
   controls, until the desired nozzle clearance is reached.
6. Repeat steps 3–5 for each remaining corner.

After leveling, run a first-layer adhesion test print. If your printer
supports it, auto-home and run bed-meshing software; keeping the bed heated
will produce more accurate results.

### Recommended Bed-Leveling Model

I use [this bed-leveling model by @Supertornado on
Printables](https://www.printables.com/model/144326). It provides a practical
first-layer adhesion test after completing the manual adjustments above.

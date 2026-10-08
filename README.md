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

## What This Reference Covers

This document will focus on the setup and manual adjustments that I have
found useful for Ender-style bedslingers. As the project grows, I plan to
include notes on the following:

* Basic first-time setup and mechanical checks
* Bed leveling and Z-offset adjustments
* First-layer testing and troubleshooting
* Useful models, upgrades, and configuration references

## How to Use This Reference

Start with the manual adjustments below before making software or hardware
changes. Once the first layer is consistent, use the linked test model to
confirm the settings. The recommendations here are based on my Ender 3 V2
Neo, so use them as a starting point and adjust them for your own machine.

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

Although simple, this model is very telling for the success rate of future prints. Look for small failures
as these often add up to much larger inconsitencies
with future larger, more complex prints.

![](./assets/photo-import-8-7-26/20261006_220210.jpg)

> Note the inconsistent extrusion here

### Mechanical adhesion test

Using the recommended model above, one useful test
may be performed using a small nylon bristeled 
brush. I prefer to perform this check as the test model
is actively printing.

![](./assets/photo-import-8-7-26/20261006_220016.jpg)

This test is perfomed by sliding the bristles
with minor tension over the first extruded layer of
the print in order to check for any inconsistent
bed adhesion. This may signify a low spot in the
bed's mechanical leveling. Follow up adjustment should
then take place.

If all looks good thus far, you may allow the print
to complete.

![](./assets/photo-import-8-7-26/20261006_220111.jpg)

One final recommendation is to look for proper spacing
between extrusions. Once again, you may use the nylon
brush or similar to inspect the adhesion between the
extruded plastic. Look for gaps or over-extrusion
that might signify the need for further tweaks to
z-offset or filament flow rate.
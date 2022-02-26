# SlideSwipe - Euclid Probe Edition
## Introduction
I liked the idea of the [SlideSwipe](https://github.com/chestwood96/SlideSwipe) method of deploying the probe but wanted to use an [Euclid Probe](https://euclidprobe.github.io/) so I have modified it to suit.
Taking probe             |  Stowing probe

## Pros and cons compared to SideSwipe
| Pro | Con |
| ---- | ---- |
| + Fully integrated | - Requires new cowling (and the accompanying rebuild of everything on it) |
| + Cables well hidden | - More complex (more parts, more steps) |
| + No loss in y area with the door closed |  |
| + Bed can't hit the arm |  |


## BOM
### Parts
- 1x MG90s Metal gear servo (the SG90 plastic gear ones work too but are not reccomended)
- 1x Euclid Probe Kit
- 1x 300mm servo extender cable (or make your own)
- 1x 1.5m of stranded wire with <1.2mm od (I tested 30awg silicone wire and 26awg ptfe wire)
- 3x 16mm piece of 4od2id PTFE tube (does not need to be the nice stuff)
- 1x 7mm piece of 4od2id PTFE tube (does not need to be the nice stuff) 
### Screws
- 7x M3x6 Socket head screw (cap head probably works too, one needs to be at least slightly attracted to magnets)
- 2x M3x8 Cap head screw
- 2x M3 nut

## Printing
All parts are designed to print in the orientation they come in and not require supports (If you have really bad overhang performance you can add a bit of support for the probe but it should not be necessary).

Designed to print in ABS at 0.4mm outer layer width and 0.2mm layer height.

I recommend ironing for the following parts, the rest can be printed without:
- Arm1
- Arm2
- ProbeCarrierTop
- ProbeCarrierBottom
- RailMountTop
- euclid mount

If you are going to do accents, I reccomend printing the following parts in the accent color:
- Arm1
- Arm2

## Cowling

This version uses the standard [Klicky Probe](https://github.com/jlas1/Klicky-Probe) cowling. I have also made a version of the klicky probe cowling for use with a mosquito.  

### Probe holder
Find the servo arm that fits the arm the best and cut off anything else on that arm if there is anything.
![ArmServoArm](Images/ArmServoArm.jpg)
![ArmServoArm2](Images/ArmServoArm2.jpg)

Zero the servo (and check that it has at least over 90° of travel and isn't a continuously rotating one) and install the chosen arm, so it points a little over 90° when at the max point (picture is the max point).
![ArmServoArm3](Images/ArmServoArm3.jpg)

Pull the servo wire through the hole.
![ArmServoMount](Images/ArmServoMount.jpg)

Insert the servo into the mount and fix it using 2 M3x6 screws
![ArmServoMount2](Images/ArmServoMount2.jpg)
![ArmServoMount3](Images/ArmServoMount3.jpg)
![ArmServoMount4](Images/ArmServoMount4.jpg)

Insert the short piece of PTFE in the left hole of "RailMountTop".
![ArmServoMount5](Images/ArmServoMount5.jpg)

Insert one of the longer pieces of ptfe into one of the holes of "Arm2"(the solid one).
![Arm1](Images/Arm1.jpg)

Put "Arm2" and "Arm1" onto the servo carrier like shown.
![Arm2](Images/Arm2.jpg)

Screw "RailMountTop" onto the servo carrier using 2 M3x6 screws.
![Arm3](Images/Arm3.jpg)

Put the other two longer pieces of ptfe into the remaining two holes in the arms.
![Arm4](Images/Arm4.jpg)

Put "ProbeCarrierTop" and "ProbeCarrierBottom" on the arms and screw them down using 2 M3x6 screws.
![Arm5](Images/Arm5.jpg)
![Arm6](Images/Arm6.jpg)

Add nuts in the pockets on the inside of the mount.
![ArmNuts](Images/ArmNuts.jpg)

That should be the physical build done.
![Arm7](Images/Arm7.jpg)

## Installation
### Installing the new cowling
The installation is the same as with the regular one, refer to the manual for that.

### Installing the probe arm
put the servo wire into the groove of the extrusion and tip the mount into it. Fix the assembly using the screws on the side.

Adjust the height to where it can grab the probe, but the arm does not hit the printhead then fix it in place.

Rout the servo wire through the slot in the front extrusion upwards into the slot of the top extrusion. The stock wire should be just long enough to pass through the panel though you'll probably have to remove the connector housing for that.

### Calibrating the servo angles
Using the servo command, find good values where the servo reliably hit the deployed and stowed position. The mechanism mechanically limits the travel but having the servo trying to push against it the whole time isn't great for it, so try to find some values that don't go way over the limits.

### Calibrating the pickup position
This should already be somewhat acurate but if it isn't find the pickup position and update the macro accordingly.

## Calibrate Z-Offset and start printing
Use your favourite method of calibrating the z-offet and start printing.
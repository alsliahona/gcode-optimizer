gcode-optimizer
===============
Copyright (c) 2014 - Andrew L. Sandoval

A command-line tool that optimizes CNC Mill and Laser Engraver gcode generated from programs like MakerCAM - also optionally converts mill gcode to laser gcode.

The image below shows a sign I made for my family opened in the "Universal gcode sender" with it's visualization view.  The left-hand side is the original MakerCAM generated file and the right-hand side is the optimized file.  Note that the blue lines all represent "rapid linear motion" (G0 codes) that indicate movement of the cutter above the surface of the material (or in the laser case, with the laser powered off.)   The more of these you have, and the further the travel, the longer it will take to produce the final product.

![alt tag](images/SideBySideComparison.png)
 
Here is an image of the Shapeoko 2 burning the image from the gcode that was optimized.  The laser is a 2 watt 445nm laser in an aluminum heatsink attached to the opposite side of spindle.  It is fixed-focused based so that Z motion is not relavent and focus is set prior to starting the operation.

![alt tag](images/LaserBurning.jpg)

The final piece looks like this:

![alt tag](images/FinalProduct.jpg)

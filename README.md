gcode-optimizer
===============
Copyright (c) 2014 - Andrew L. Sandoval  (See LICENSE file for details.)

A command-line tool that optimizes CNC Mill and Laser Engraver gcode generated from programs like MakerCAM - also optionally converts mill gcode to laser gcode.

The image below shows a sign I made for my family opened in the "Universal gcode sender" with it's visualization view.  The left-hand side is the original MakerCAM generated file and the right-hand side is the optimized file.  Note that the blue lines all represent "rapid linear motion" (G0 codes) that indicate movement of the cutter above the surface of the material (or in the laser case, with the laser powered off.)   The more of these you have, and the further the travel, the longer it will take to produce the final product.

![Alt text](https://raw.githubusercontent.com/alsliahona/gcode-optimizer/master/images/SideBySideComparison.PNG "Side-by-Side")
 
Here is an image of the Shapeoko 2 burning the image from the gcode that was optimized.  The laser is a 2 watt 445nm laser in an aluminum heatsink attached to the opposite side of spindle.  It is fixed-focused based so that Z motion is not relavent and focus is set prior to starting the operation.

![Alt text](https://raw.githubusercontent.com/alsliahona/gcode-optimizer/master/images/LaserBurning.JPG "Burning")

The final piece looks like this:

![Alt text](https://raw.githubusercontent.com/alsliahona/gcode-optimizer/master/images/FinishedProduct.JPG "Finished Product")

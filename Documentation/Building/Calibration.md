# Calibration

While general values for the number of steps per millimeter will give you decent accuracy, it is necessary to calibrate and change the steps per millimeter for the best accuracy. There are many online guides for calibrating the steps/mm for 3D printers, such as this one found here at All3DP (https://all3dp.com/2/extruder-calibration-6-easy-steps-2/). However, we will have to change a few things to calibrate the syringe pump, since it is a little different from a 3D printer.

# Supplies Needed

- Scale
- Water Container
- Distilled Water
- Needle or Pipette Tip
- Tubing

# Steps

1. Plug in syringe pump
2. Fill syringe with distilled water
3. Attach tubing to the pump with a needle/pipette tip on the other end of the tubing
<p align="left">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6247.JPG" width="200"/>
<h6 align="left">Attached a pipette tip for calibration</h6>

4. Prime the pump by pumping water till it starts to drip out of the needle
5. Place water container on the scale and tare the scale
6. Pump out 5 mL of water into the container and record the weight
7. Tare the scale again and repeat step 6 five more times
8. Take an average of all six measurements

The density of pure water is 1 gram per cubic centimeter (g/cm^3). Since 1 mL is one cubic centimeter, we can calculate exactly how much water was pumped out each time and adjust accordingly.

For example we will use 4.8 grams as our average.

Determine how many steps per millimeter the motor took to pump out 4.8 g of water. Multiply the number of steps (This can be found under Control > Motion > Steps/mm) by the number of milliliters that were supposed to be extruded.

  [Steps/mm] x 5 mL = Steps taken

Then we will use the number of steps taken to determine the new number of steps needed.

  [Steps taken] / [Average weight in grams] = [New steps per millimeter value]

The combined equation is:

  [Original Steps/mm] x [Volume supposed to be pumped] / [Averaged weight in grams] = [New steps/mm value]

The new steps/mm value can then be changed by following the same path, and then twisting the control knob until the desired value is set. It can also be changed by changing the appropriate value in the firmware.  

NOTE: If the new steps/mm value is not saved by going Control > Store Settings the new steps/mm value will have to be entered every time that the pump is turned on.

It may be necessary to perform this calibration multiple times to ensure that the calibration is correct. It is also advisable to perform the calibration for all three main volumes (5, 1, 0.5 mL) and then averaging the steps/mm value calculated for each volume. This is because the steps/mm required often increase as smaller volumes are extruded.

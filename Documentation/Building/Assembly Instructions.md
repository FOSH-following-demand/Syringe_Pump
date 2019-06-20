# Steps

1. Purchase all of the parts from the [Electrical bill of materials](https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Hardware/Bill_of_Materials/Electrical_BOM.csv) and the [Mechanical bill of materials](https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Hardware/Bill_of_Materials/Mechanical_BOM.csv)
1. 3D print all the necessary [parts](https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Hardware/Frame/3D_Printed_Parts/3D_Printed_Parts.csv)
1. Assemble the syringe pump body by following the directions found [here](https://www.sciencedirect.com/science/article/pii/S2468067217300822#!). Please refer to [troubleshooting](Troubleshooting.md) for any problems that you encounter as we discovered a few quirks with the assembly described in the link.
1. Remove the control knob from the Smart Display

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6283.jpg" width="500"/>
<h6 align="center">Removed control knob</h6>

1. Attach the MKS-Base v1.6 and the Smart Display to the controller cabinet using M3 X 8 screws
  -Note: Depending on the tolerances and nuances of every 3D printer, and different part manufacturers, the fit of the MKS-Base and Smart Display might be a little off. Only two screws are necessary to hold the parts in place, and some of the screen hole may need to be shaved down with a razor blade for the screen to fit.
1. Replace the control knob

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6284.jpg" width="500"/>
<h6 align="center">Replaced control knob</h6>

1. If the power supply has an extendable plug, attach it to the board and feed the wires through the power port, otherwise cut off the end of the power supply, strip the wires, and attach the exposed leads to the board

  <p align="center">
  <img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6279.jpg" width="500"/>
  <h6 align="center">MKS-Base in the case with power supply attached</h6>
  <p align="center">
  <img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6280.jpg" width="500"/>
  <h6 align="center">Fasten the screen to the case</h6>

1. Place syringe pump body on the top of the case. Put two M3 X 45 screws through the two holes by the bearing and feed them through the last slot on the case. Attach with washers and M3 nuts. Note: I did not have any M3 nuts on hand, so I improvised with some larger nuts to hold mine in place.
1. Drill two holes with the 7/64th drill bit towards the front of the pump body, and drill through the pump and the case. Push two M3 X 45 screws in and fasten with M3 nuts and washers. Note: If you drill too close to the edge of the case, you will be unable to put a nut and washer on that screw.

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6287.JPG" width="500"/>
<h6 align="center">Screws drilled and attached through the pump body</h6>
<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6281%20(1).JPG" width="500"/>
<h6 align="center">Inside of case, where the body is attached to the electronics case</h6>

1. Plug the screen cables in and plug the stepper motor cable in to the E0 port as show in the picture

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6282.jpg" width="500"/>
<h6 align="center">Cables plugged into the MKS-Base</h6>

1. Plug the other end of the screen cable into the Smart Display. Ensure that the EXP1 and EXP2 ports on the display are connected to the same ports on the board

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6285.jpg" width="500"/>
<h6 align="center">Cables plugged into the Smart Display</h6>

1. Feed the stepper motor cable through one of the slots in the back of the case, and connect it to the stepper motor on the pump body

<p align="center">
<img src="https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Photos/IMG_6286.jpg" width="500"/>
<h6 align="center">Stepper motor cable connected</h6>

1. Plug the power supply in and ensure that everything turns on and that the stepper motor rotates
1. Close the case
1. Connect the computer cable to the port on the back of the case, and connect the USB to your computer.
1. Using the [Arduino IDE](https://www.arduino.cc/en/Main/Software) upload the [firmware](https://github.com/FOSH-following-demand/Syringe_Pump/tree/master/software/MCU/Firmware/Syringe_Pump) by following these [instructions](https://www.arduino.cc/en/Guide/ArduinoMega2560#toc2)
1. Follow the [instructions](https://github.com/FOSH-following-demand/Syringe_Pump/blob/master/Documentation/Usage/Getting%20Started) to start using your syringe pump
1. [Calibrate](Calibration.md) your syringe pump
1. Do awesome science!!!

# TTL Controller for High-Speed Microscopy 

<img src="https://github.com/mariavmukhina/TTL_Controller_for_Microscope/blob/main/images/controller-small.jpg">  

An inexpensive Transistor-Transistor Logic (TTL) controller consisting of Arduino and custom-made printed board that listens to firing TTL pulse from camera and generates up to 8 TTL output pulses. [Software for the controller](https://github.com/mariavmukhina/ScopeScript/tree/main/hardwareControl/piezoController/arduinoFirmware) in Arduino programming language allows to synchronize camera image acquisition with turning on epi or brightfield illumination, moving the piezoelectric Z stage, and applying mechanical deformations to the sample with nanomanipulator, as shown below. 

The unique feature of the controller is fast aqcuisition in 3D, which is achieved by sending the full "recipe" for a 3D stack to the piezoelectric Z stage before the acquisition starts. In the test experiments, the controller coupled to PI NanoZ stage and sCMOS Hamamatsu Flash 4.0 V3 camera enabled acquisition over a volume up to 133x133x100 µm^3 in 1.42 sec that is equivalent to the rate of 4.2x10^8 voxels/sec (with 10 msec exposure per z slice and 1 µm axial resolution). 

The provided files contain design files for the custom printed circuit board (PCB, can be ordered from https://oshpark.com/), the parts list for the PCB, and soldering and assembling instructions.

<img src="https://github.com/mariavmukhina/TTL_Controller_for_Microscope/blob/main/images/TTL%20triggering%20scheme.png" >

Have a question? Get in touch!
You can email me at mmukhina@fas.harvard.edu, or raise a support [issue](https://github.com/mariavmukhina/TTL_Controller_for_Microscope/issues/new?assignees=mariavmukhina&labels=help+wanted&template=support-request.md&title=%5BSUPPORT%5D).

Frederick Chang designed and programmed the controller (2017). Maria Mukhina introduced changes to the board design to add additional epi channel and new TTL output for optional peripheral device (2020). 

## Kleckner Lab Acknowledgement

Please acknowledge the Kleckner Lab in your publications. An appropriate wording would be: "The TTL controller design was provided by the laboratory of Nancy Kleckner at Harvard University, funded in part by National Institutes of Health (NIH) grant R35GM136322."




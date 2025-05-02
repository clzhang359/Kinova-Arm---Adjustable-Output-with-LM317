# PCB for Adjusting the Voltage Output from the Kinova Arm with an LM317
Last Updated: 2025/05/02

This repo was made by Connie L. Zhang at Georgia Tech at the SAFE Robotics Lab as a part of the Farmhand Project.

The 24V output of the Kinova Arm was too much for the microscope's motor (12V/1.5A), so the LM317 was applied to decrease the output voltage. This specific device was chosen since (a) it was available at the HIVE makerspace and (b) I have used this in a previous class.

This PCB Design was made in KiCAD.

The LM317 [1] is an adjustable voltage regulator that can input up to 40V and output anywhere between the provided input and 1.25V and up to 1.5A.

## Should I use this PCB for my project with my Kinova Arm?

Firstly, how much voltage and current does your voltage require?
- If it requries **less than 24V & less than 1.5A**, then yes, you can use this PCB.
- If it requries **less than 1.25V**, then **do not** use this PCB design.
- If it requires **more than 1.5A**, then **do not** use this PCB design.
- If it requires **more than 24V & less than 1.5A**, then **do not** use the LM317 or this PCB.

## Reference: 
[1] https://www.ti.com/lit/ds/symlink/lm117.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1726162841584&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm117

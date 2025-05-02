# PCB for Adjusting the Voltage Output from the Kinova Arm End Effector with an LM317
_This repo was made by Connie L. Zhang at Georgia Tech at the SAFE Robotics Lab as a part of the Farmhand Project._

_Last Updated: 2025/05/02_

The 24V output of the Kinova Arm was too much for the microscope's motor (12V/1.5A), so the LM317 was applied to decrease the output voltage.

This PCB Design was made in KiCAD, and all design files can be found in the "kinova_arm_pcb_adjust" branch. The "fabexport_pwrpcb.zip" contains all the PCB manufacturing files.

This PCB goes on the Kinova Arm's End Effector and matches the provided pinout as shown below from the manual: 

![End Effector Pinout](/../main/images/kinova_pinout.png)

## Why the LM317?

This specific device was chosen since (a) it was available at the HIVE makerspace, (b) I have used this in a previous class, and (c) the project fit the application.

The [LM317]([https://www.ti.com/lit/ds/symlink/lm117.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1726162841584&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm117](https://www.st.com/resource/en/datasheet/lm217.pdf)) is an adjustable voltage regulator that can input up to 40V and output anywhere between the provided input and 1.25V and up to 1.5A.

## Should I use this PCB for my project with my Kinova Arm?

Firstly, how much voltage and current does your voltage require?
- If it requries **less than 24V & less than 1.5A**, then yes, you can use this PCB.
- If it requries **less than 1.25V**, then **do not** use this PCB design.
- If it requires **more than 1.5A**, then **do not** use this PCB design.
- If it requires **more than 24V & less than 1.5A**, then **do not** use the LM317 or this PCB.

## I can use this PCB! Yay! 😄 Now what?


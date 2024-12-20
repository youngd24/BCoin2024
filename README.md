# BCoin2024
BurbSec Challenge Coin 2024

What's the challenge? Show up to a meetup! That's it, show up and new attendees get one.

## Front
![BCoin Front](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-front.jpg)

## Back
![BCoin Back](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-back.jpg)

## Schematic
![Schematic](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-schematic.jpg)

## Hacking it

If you want to adjust the rate at which the LED's flash around the edge you can swap out the R1/R2/C1 components that drive the 555 (astable) timer circuit. The value they're set to in the current form will drive them at 4.8 Hz, current values are:

R1 - 10k - 0603 size\
R2 - 10k - 0603 size\
C1 - 10uF - 0805 size

DigiKey has a great tool to calculate the values [here](https://www.digikey.com/en/resources/conversion-calculators/conversion-calculator-555-timer), just be sure to select the "astable" one. Order some options from them, break out the soldering iron and hack it up!

## Modifying it

Feel free to change whatever you'd like in the design, circuit or PCB. Make sure you run the ERC against the schematic as well as the DRC against the PCB, this will help catch any basic errors you may have introduced. Once you're ready use [these instructions](https://www.pcbway.com/blog/help_center/How_to_Generate_Gerber_and_Drill_Files_in_KiCad_7_0_ab0d12bb.html) to generate the Gerber and drill files needed for manufacturing.

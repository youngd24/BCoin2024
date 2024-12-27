# BCoin2024
BurbSec Challenge Coin 2024

What's the challenge? Show up to a meetup! That's it, show up and new attendees get one.

## Why?

I've organized the South instance of BurbSec for coming up on a decace, I've always wanted something to be able to give new attendees as a sort of "thanks for coming". At the same time I wanted them to take something away, something to help them remember us, and to include the basic information about the Meetup itself, when, where and so on. While I was at it, why not have it be educational as well, in this case one of the most fundamentally basic of electronics circuits: the venerable 555 timer. I wanted it to be small, low cost, easy to modify for others, and dead simple to make. This version is 50mm in diameter and approximately 5mm thick, including the CR2016 battery, so it will fit in many (most) of the clear acrylic "challenge coin" or "collector coin" type cases. Double check on the thickness of whatever you find, that's where it gets to be sort of painful and expensive. A thinner, 40mm version is planned to help ease that challenge.

## How?

At the core is a basic astable 555 timer, programmed via the RC circuit to be around 4Hz, which in turn drives a decade counter to the perimeter LED's. It's a "chaser" sort of circuit, they light up in order, that's it, dead simple. It's driven from a single CR2016 battery, though the pads fit a CR2032 holder as well. The components on the board are good down to around 2.6V so the battery should hold up for a bit, how long though, who knows, this thing isn't meant to run all day, it's a token.

## Schematic
![Schematic](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-schematic.jpg)

## Front
![BCoin Front](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-front.jpg)

## Back
![BCoin Back](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.4-back.jpg)

## Assembled
![BCoin Assembled](https://github.com/youngd24/BCoin2024/blob/main/assets/BCoin2024-v0.3_assembled.JPG)

## Hacking it

If you want to adjust the rate at which the LED's flash around the edge you can swap out the R1/R2/C1 components that drive the 555 (astable) timer circuit. The value they're set to in the current form will drive them at 4.8 Hz, current values are:

R1 - 10k - 0603 size\
R2 - 10k - 0603 size\
C1 - 10uF - 0805 size

DigiKey has a great tool to calculate the values [here](https://www.digikey.com/en/resources/conversion-calculators/conversion-calculator-555-timer), just be sure to select the "astable" one. Order some options from them, break out the soldering iron and hack it up!

## Modifying it

Feel free to change whatever you'd like in the design, circuit or PCB. Make sure you run the ERC against the schematic as well as the DRC against the PCB, this will help catch any basic errors you may have introduced. Once you're ready use [these instructions](https://www.pcbway.com/blog/help_center/How_to_Generate_Gerber_and_Drill_Files_in_KiCad_7_0_ab0d12bb.html) to generate the Gerber and drill files needed for manufacturing.

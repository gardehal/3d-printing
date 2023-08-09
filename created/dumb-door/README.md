# Dumb door

Like a smart door, but dumb. Does not require invasive installation.

## TODO

- API on PICO that receives secure calls over LAN to change lock state. Login/simple user functionality. Some basic stats and logs like last (100?) change datetime and by who, number of lock calls, number of unlocks calls, ...
- Charts and final documentation.
- Guide for print and assembly

## Part list

- 2x 18650 Lithium-Ion rechargeable batteries (with tip)
- 1x NEMA-17 step-motor
- 1x motor driver
- 1x JST PH 4-Pin cable (for motor)
- 1x Raspberry Pi Pico W
- 1x on/off switch
- 1x button (optional)
- 1x multicolour LED (optional)
- 1x half-size breadboard (optional)
- 2x zip ties 3mm x 1mm x 80+mm
- 3x M4 x 12mm bolts/screws + nuts
- 4x M5 x 12mm bolts/screws + nuts (2x is fine)
- 1x push spring (7.5mm x 13mm), cut in half
- solid core wires
- some string (optional)

## Setup guide

## Assembly

TODO
pics of frame on door, assembled individual parts, final assembly

## Circuit diagrams

TODO

## Retrospect

#### Worries
electronics: voltages etc. enough for motor and power to pico?
battery charge only lasting a few days tops (annoying for a real world product)
non-elegant design, batteries could be put below handle etc. but would make it more complicated to adapt to other doors

#### Good
hinges
brackets + modular design
fun
incorporated other parts like nuts/bolts/switch/buttons
potentially usable
pins worked well

#### Bad
initial design was bad, did not think it though


#### Neutral
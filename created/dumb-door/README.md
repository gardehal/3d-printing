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

1. Load frame-upper and frame-lower into a CAD with a rough 1:1 drawing of your handle and lock and check the following:
  - frame-upper handle shape and size
  - frame-lower fit with locking mechanism, height and width wise
  - lock-adapter fits your locking mechanism
  - lock gear and motor gears fit and get a good grip
1. Print the following parts (optional order, but recommended so you can multitask with steps 3+):
  - 1x frame-upper
  - 1x frame-lower
  - 1x lock-adapter
  - 1x battery-case
  - 1x brain-case
  - 1x lock-gear
  - 2x lock-gear-pin
  - 1x motor-gear
  - 1x motor-case
  - 2x motor-case-clip
  - 1x brain-lid
  - 1x battery-lid
1. Check that these parts physically fit and can be assembled with your setup:
  - frame-upper can be put over your handle and sits reasonably well when assembled as shown in the graphics
  - frame-lower can be attached to frame-upper and is flat towards the door
  - lock-adapter can be attached to the locking mechanism without any other movement than rotating with the lock
1. Adjust frames or gears as appropriate
1. Assemble the parts:
  - battery-case - using springs and wires to connect the batteries in series
  - brain case - attach LED, on/off switch, open/lock button, assemble breadboard with parts as shown in the graphics, wire everything up

...
assemble motor + case + gear
attach lock adapter + gear
nuts and bolts and lids
attach everything to frame and secure to upper frame on the door

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
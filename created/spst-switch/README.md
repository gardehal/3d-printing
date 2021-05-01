# Single Pole Single Throw (SPST) Switch

A home made switch for completeing a curcit.

**WARNING: this item may constitute a fire hazard. Use at your own risk!**

--- 

## Development

- Measurements given as [height]x[length]x[width]
- Arrow with a name ("-> [name]") indicate a parts or objects new name
- X, Y, and Z axes abbreviated to just "X", "Y", or "Z".

### General plan

A switch with a binary on/off state, flipping the lever will change the state, connecting or disconnecting the wires and completing or breaking a circuit.
There is no need to over-engineer this, all needed, in theory, is a housing, the lever itself, 2 wires, some glue, and a wire cutter or something sharp to fray the wires.
Bonus points for soldering to increase contact surfaces.
A cursory search did not yeld any information about standardized components or sizes, so there wasn't much thought put into it for development.

Rough plans drawn in paint:
![Image of plans](./001-spst-switch-plans.png)

### Version 0.0.1

#### Part-A

Housing

1. Created a box, main housing, 20x20x28 mm -> A1
1. Created a box, housing lip, 2x22x30 mm -> A2
1. Created a negative space box, main housing space, 17x17x23.8 mm -> A-ns1
1. Align A1, A2, A-ns1 around X and Y, all top common Z
1. Combine -> A1
1. Created a negative space cylinder, openings for wires, 40x2x2 mm -> A-ns2
1. Align A1, A-ns2 around X and Y, all bottom common Z
1. Move A-ns2 +2 mm Z
1. Combine -> A1


1. Created a negative space cylinder, slots for hinge where Part-B rotates around, 40x2x2 mm -> A-ns3
1. Created a negative space box, slots where Part-B can lock position, 2x4x24.8 mm -> A-ns4
1. 

#### Part-B

Switch


---

#### Part-C

Wire clamps
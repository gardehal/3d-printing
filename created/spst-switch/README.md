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

3 parts:
1. Part-A - Main housing
1. Part-B - the moving switch
1. Part-C (optional) - Clamps to keep wires in place

Rough plans drawn in paint:
![Image of plans](./001-spst-switch-plans.png)

### Version 0.0.1

#### Part-A

1. Created box, main housing, 20x20x28 mm -> A1
1. Created box, housing lip, 2x22x30 mm -> A2
1. Created negative space box, main housing space, 17x17x23.8 mm -> A-ns1
1. Aligned A1, A2, A-ns1 around X and Y, all top common Z
1. Combined -> A1
1. Created negative space cylinder, openings for wires, 40x2x2 mm -> A-ns2
1. Aligned A1, A-ns2 around X and Y, all bottom common Z
1. Moved A-ns2 +2 mm Z
1. Combine -> A1
1. Created negative space cylinder, slots for hinge where Part-B rotates around, 40x2x2 mm -> A-ns3
1. Created negative space box, slots where Part-B can lock position, 2x4x24.8 mm -> A-ns4
1. Aligned A1, A-ns3, A-ns4 around X and Y.
1. Moved A-ns3, A-ns4 +10 mm Z
1. Combine -> A1
1. Printed A1

#### Part-B

1. Created box, switch body, 10x23.8x17 mm -> B1
1. Created negative space half cylinder, arch on top of switch, 5x17x23.8 mm -> B-ns1
1. Created negative space box, angled faces on sides of switch, 20x20x20 -> B-ns2
1. Rotated B-ns2 -22.5 degrees around Y
1. Copied B-ns2 -> B-ns3
1. Rotated B-ns3 +90 degrees around X
1. Copied and combined (toggle negative space, combine) A-ns3, A-ns4 -> B2
1. Aligned all parts around X and Y, all bottom common Z
1. Aligned B1, B-ns1 to top shared Z
1. Moved B-ns2, B-ns3 +2 mm Z
1. Moved B-ns2 -18.5 mm X
1. Moved B-ns3 +18.5 mm X
1. Combine -> B1
1. Printed B1

#### Review

- Part-A
  - Can be overall smaller.
  - Add holes though floor for more wire options.
  - Thinner walls.
  - Should have a lip inside shaped as an upside-down V, so the switch cannot pivot too far down.
  - Pivot point could be slightly higher.
- Part-B
  - Part B should be smaller, 0.5 mm on Y parallel (short sides) so it does not rub against Part-A so much.
  - Curve could be slightly steeper, but the middle is flush with Part-A.
  - 1 and 0 on switch.
- B2
  - Combining A-ns3, A-ns4 was an error, A-ns3 should be used this way, but A-ns4 should be split and the notches rounded, then used on the sloped faces, rather than the vertical faces so Part-B can pivot and lock in place. For testing v0.0.1, these notches were simply cut off after print, before putting the parts together.

---

### Version 0.0.2

#### Part-A

#### Part-B

1. Used Part-B v0.0.1 as base
1. Rotated B-ns2 and B-ns3 further, now a total of 30 degrees tilt
1. Moved B-ns2 and B-ns3 closer tot he part, now 15.5 mm from the collective X
1. Deleted A-ns4 from B2, not is just the hinge -> B2
1. Moved B2 +2 mm Z
1. Created two half cylinders, for notches to lock switch in position, 1x4x2 mm -> B3-1, B3-2
1. Rotated B3-1 +30 degrees around Z
1. Rotated B3-2 -30 degrees around Z
1. Moved B3-1 to middle of sloped face created by B1-ns2
1. Moved B3-2 to middle of sloped face created by B1-ns3
1. Combined all parts
1. Printed part

#### Part-C

#### Review

---

### Version 0.0.3

#### Part-A
#### Part-B
#### Part-C
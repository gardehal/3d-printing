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

1. Used Part-A v0.0.1 as base
1. Added a 1 mm thin wall 4 mm up from bottom on inside of housing
1. Removed lip around top for faster print
1. Removed bottom half for faster print
1. Printed part

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

#### Review

- Wall inside Part-A was not connected to the actual housing, slicer ignored this wall.
- It's a good idea to prototype with smaller segments before pringint the whole part, print of Part-A 0.0.2 was 60% faster than 0.0.1.

---

### Version 0.0.3

#### Part-A

1. Used Part-A v0.0.2 as base, removed inner walls.
1. Changed size of A-ns1 to 13x26x18 mm
1. Changed size of A-ns3 to 2x2x19 mm
1. Moved hinge slots (A-ns3) to max common Z with A1, then -1 mm Z
1. Printed part

#### Part-B

1. Created half cylinder, switch face, 10x26x18 mm -> B1
1. Created negative space box, switch face, 10x26x18 mm -> B1-ns1
1. Moved B1-ns1 +5 mm Z
1. Align center X Y Z
1. Combined -> B1
1. Copied B1 -> B2
1. Rotated B1 +180 degrees around Y
1. Moved B2 +5 mm Z
1. Created negative space box, B2 surplus material, 20x20x20 mm -> B2-ns1
1. Align center X Y Z
1. Combined B2, B2-ns1 -> B2
1. Copied A-ns3 from Part-A -> B3
1. Align center X Y Z
1. Moved B3 +3 mm
1. Created two half cylinder, latches, 1x2x4 mm -> B4, B5
1. Placed B4, B5 on B2
1. Rotated B4 +75 degrees around Y
1. Moved B4 -16 mm X
1. Made sure B4 sits 0.5 mm out of B2
1. Mirrored last three steps with B5
1. Combined -> B1
1. Printed part

#### Review

- Part-A walls too thin and flexible, 2 mm should be fine, maybe lip and floor helps, but Part-A v0.0.2 is strong enough (3 mm walls) without them.
- Part-B fits better with rounded sides, slots for hinge and locking notches needs to be moved up, preferably the end of the active side should be close to flush with Part-A.

---

### Version 0.0.4

#### Part-A

1. Used Part-A v0.0.3 as base
1. Changed size of A-ns3 to 2x4x30 mm
1. Changed size of A-ns4 to 2x4x24.8 mm
1. Created a copy of A1 -> A2
1. Changed size of A2 to 2x22x30 mm
1. Aligned A1 and A2 with common top Z
1. Moved A2 -2 mm Z
1. Combined -> A1
1. Printed part

#### Part-B

1. Used Part-B v0.0.3 as base
1. Moved B3 and B2-ns1 +2 mm Z
1. Combined -> B1
1. Printed part

#### Review

- Part-A still weak even with brace, should have 3 mm thick walls.
- Part-B too large, shaving off 0.5 to 1 mm width-wise seems like it should be enough.
- Part-B should be more hollow to reduce material.
- Part-B should can have hollow "1" and "0" markings, making them extruding is difficult to print.
- Hinge and notches seem to be in a good position, does not seem to let anything though the off-side when on.

---

### Version 0.0.5

#### Part-A

1. Used Part-A v0.0.4 as base
1. Changed size of A-ns3 to 17x17x25 mm
1. Removed temporary unnamed brace
1. Combined -> A1
1. Printed part

#### Part-B

1. Used Part-B v0.0.4 as base
1. Shrunk all parts but A-ns4 1.5 mm Y
1. Shrunk all parts but A-ns3 1 mm X
1. Combined -> B1
1. Printed part

#### Review
- Forgot numbers again
- The switch works as expected, but it's hard to tell if the notches on the sides enter the slots and exactly when they do.
- Width of Part-B could be reduced slightly more, less than 0.5 mm. Notches seem to scratch on wall of Part-A.
- Combining scratching with the missing event of a spring or mechanical even to push the switch away from a middle-position, the project seems somewhat pointless as it won't be as useful as even a temporary replacement for an actual switch.

---
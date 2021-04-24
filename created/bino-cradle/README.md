# Binocular cradle

Two clip-on cradles that come together to hold to binoculars, Optic-A and Optic-B.

## Version 1
### Part-A

Part-A is for the thick cylinder. Made for Optic-A which has a loose, firm-rubber cover, 29 mm diameter It measures 29x29x80 mm.

- Created representation of Optic-A as per specification.
- Copied object (Optic-A-Copy) (29x29x80 mm).
- Created a cylinder (Part-A) 4 mm larger in diameter than Optic-A-Copy, 40 mm tall (32x32x40 mm).
  - Aligned Part-A and Optic-A-Copy along X and Y axis, set Z to 0.
  - Moved Optic-A-Copy +3 mm along X axis.
  - Made Optic-A-Copy negative to remove part of Part-A it overlapped with.
  - Combined objects, removing a space for Optic-A to sit in.
- Copied M4 (7x8x3.5 mm) nut (M4n-A1) from metric-screws project.
- Copied M4n-A1 twice (M4n-A2, M4n-A3) expanded hole to 5 mm so M4 screws can rotate freely.
- Align M4n-A2 and M4n-A3.
- Created a negative cylinder (B-M4n-space) to make holes for M4n attached to Part-B.
  - Set B-M4n-space to 8x8x20 mm.
  - Align B-M4n-space, M4n-A2, and M4n-A3 along all 3 axes (M4n-A2+).
  - Did NOT combine objects.
- Aligned Part-A and M4n-A2+ along X and Y axis, set Z to 0.
- Moved M4n-A2+ -12.5 mm along X axis so the lines of Part-A was not visible inside the nuts.
- Combined B-M4n-space with Part-A to remove space for Part-B nuts.
- Moved M4n-A2 -3.5 mm along Y axis.
- Moved M4n-A3 +3.5 mm along Y axis. There was now a 3.5 mm slot between the nuts for Part-Bs M4n-B.
- Combined M4n-B and Part-B. Made sure the nuts and part was connected.
- Aligned M4n-A1 with Part-A along X and Y axis, aligned M4n-A1 to top of Part-A.
- Moved M4n-A1 -12 mm along X axis.
- Rotated M4n-A1 +10 degrees. 
- Combined Part-A and M4n-A1.
- Printed Part-A.

### Part-B

Part-B is for the thin cylinder. Made for Optic-B which has a hard metal surface, 24 mm diameter. It measures 24x24x100 mm.

- Created representation of Optic-B as per specification.
- Copied object (Optic-B-Copy), shrunk diameter by 1 mm to 23 mm (23x23x100 mm).
- Created a cylinder (Part-B) 4 mm larger in diameter than Optic-B-Copy, 40 mm tall (23x23x40 mm).
  - Aligned Part-B and Optic-B-Copy along X and Y axis, set Z to 0.
  - Moved Optic-B-Copy -3 mm along X axis.
  - Made Optic-B-Copy negative to remove part of Part-B it overlapped with.
  - Combined objects, removing a space for Optic-B to sit in.
- Copied M4 nut (M4n-B) used in Part-A (M4n-A2).
- Created a negative cylinder (A-M4n-space) to make holes for M4n attached to Part-A.
  - Set A-M4n-space to 8x8x20 mm.
  - Align A-M4n-space and M4n-B along all 3 axes (M4n-B+).
  - Did NOT combine objects.
- Aligned Part-B and M4n-B+ along X and Y axis, set Z to 0.
- Moved M4n-B+ +10.5 mm along X axis so the lines of Part-B was not visible inside the nut.
- Combined A-M4n-space with Part-B to remove space for Part-A nuts.
- Combined M4n-B and Part-B. Made sure the nuts and part was connected.
- Printed Part-B.

### Part-C

Part-C are 2 M4 screws and a M4 nut to keep Part-A and Part-B together and adjust the angle of elevation.

- Copied two M4-14 screws (M4-C1, M4-C2) and one M4 nut (M4n-C) from metric screws project.
- Printed Part-C.  

### Conclusions

- Part-A
  - Optic-A is easier to take out of the Part-A than to put in, the loose rubber cover gives in when Optic-A is forced into it's cradle. 
  - Once in it takes a great deal of force to rotate and even more to slide the optic up and down in the cradle.
  - Clip on cradles may not be the best option for softer surfaces. This is a special case with a high grip rubber around a smooth metal cylinder.
  - The overhanging M4n-A1 nut wasn't as large of a problem as first assumed it does work, but result wouldn't hurt from having more support during printing from slope under, more easing the curve.
  - There is a lip on Part-A under the cut out space for Part-Bs M4n-B that catches on the nut. Can be removed.
- Part-B
  - Optic-B fits snugly in Part-B, it can be rotated and moved up and down with some force but will not do so by itself, even when experiencing sudden deceleration. 
  - The objects can snap apart and together with great the slightly more force and is quite satisfying. 
  - For hard surfaces, make the cradle area slightly smaller (1 mm for 24 diameter) to increase grip. Corners could be rounded to reduce likelihood of snagging onto loose fabric.

- Part-As M4n-A1 nut was designed to elevate the angle between the but it's hard to reach, not long enough, and/or not elevate enough. 
  - A better solution might be 2 longer screws on each side of Part-A with a slight angle towards Part-B, pushing directly down. Less directional stress on screw with the option of small amount of roll on Part-A.
- Enlarged nuts M4n-A2, M4n-A3, M4n-B are larger than necessary, allows for yaw and elevation of parts A and B.
- Action likely would be smoother if M4n-A2, M4n-A3, M4n-B were circles, not hexagonal shapes.
- Can add a M8 nut for tripod or clamp setup later.
- When designing, be careful when combining.
  - Combine objects to make the smaller parts of a build, but don't all the sub-parts until right before printing.
  - Not combining as you go makes these separate sub-parts easier to adjust other parts later.
  - Lock sub-parts in place to stop accidentally changing them.
  - Save the build uncombined, only combine to export and print.

## Version 2
### Part-A

Using Part-A v1 as starting point.

- Copied Part-A (Part-A-v2)
- Locked Part-A-v2 in place.
- Copied M8 nut (M8n-A) from metrics screws project.
- Aligned Part-A-v2 and M8n-A.
- Rotated M8n-A 90 degrees so hole aligns with Y axis.
- Moved M8n-A -14 mm Y, -2 mm X so the nut is exposed on the side (Remember to add support structures).
- Alined Part-A-v2 and M8n-A with the top of Part-A-v2, then moved M8n-A 1 mm down.
- Copied negative space of Part-A-v2 (Part-A-v2-negative), moved it -2 mm Y.
- Combined Part-A-v2-negative and M8n-A to hide nut inside cradle.
- Locked M8n-A in place.
- Created new hinge for screw with circle instead of hex nut.
  - Created cylinder (Part-A-H), set size to 8x8x3.5 mm.
  - Created negative space cylinder for screw (Part-A-H-negative) as 4.5x4.5x5 mm.
  - Aligned Part-A-H-negative and Part-A-H along middle of all axes.
  - Combined parts.
- Created negative space cylinder (Part-B-H-negative) for Part-B hinge, 8x8x20 mm.
- Aligned Part-A-v2, Part-B-H-negative and Part-A-H along middle X and Y axis, bottom of Z axis.
- Moved Part-B-H-negative and Part-A-H +14.5 mm along X.
- Combined Part-B-H-negative and Part-A-v2.
- Combined Part-A-H and Part-A-v2.
- Created a box (Part-A-H-gap), 6x3.5x1 mm to fill cap under Part-A-H.
- Aligned Part-A-v2 and Part-A-H-gap along middle X and Y axis, bottom of Z axis.
- Moved Part-A-H-gap +8 mm on X.
- Combined Part-A-H-gap and Part-A-v2.
- Printed Part-A-v2. 
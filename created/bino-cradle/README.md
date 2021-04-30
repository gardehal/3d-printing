# Binocular cradle

Two clip-on cradles that come together to hold to binoculars, Optic-A and Optic-B.

## Version 1
### Part-A

Part-A is the thick cylinder. Made for Optic-A which has a loose, firm-rubber cover, 29 mm diameter It measures 29x29x80 mm.

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

Part-B is the thin cylinder. Made for Optic-B which has a hard metal surface, 24 mm diameter. It measures 24x24x100 mm.

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

### Part-D

Part-D is the ball-joint used to connect the M8n port on Part-B-v2 to Part-E, which is the a clamp that can be used to attach the mount to a wall or table.

- Part-D1
  - Created a sphere (D1-S), 20x20x20 mm.
  - Copied M8n form metric screws project (D1-M8n).
  - Created negative space cylinder (D1-NS), 10x10x10 mm.
  - Aligned D1-S, D1-M8n, and D1-NS along X and Y, both 0 mm Z.
  - Combined D1-S and D1-NS (D1-S).
  - COmbined D1-S and D1-M8n.
  - Printed Part-D1.
- Part-D2
  - Copied two M8n (D2-M8n-1, D2-M8n-2).
  - Created a sphere (D2-D1-ns), 20.5x20.5x20.5 mm (0.5 mm larger than D1 sphere).
  - Made D2-D1-ns negative space and locked it in place.
  - Aligned D2-M8n-1, D2-M8n-2, D2-D1-ns around X and Y, set all part to 0 Z.
  - Moved D2-M8n-1 -10 mm X.
  - Moved D2-M8n-2 +10 mm X.
  - Combined D2-M8n-1 and D2-M8n-2 (D2-M8n).
  - Aligned D2-M8n and D2-D1-ns around center of D2-D1-ns Z.
  - Locked D2-M8n in place.
  - Copied an M8-24 (D2-M8) nut from metric screws project.
  - Aligned D2-M8 with D2-D1-ns.
  - Moved D2-M8 +10 mm Z.
  - Locked D2-M8 in place.
  - Created a ring (D2-R1) with rounded top and bottom, about 2 mm thick wall, 10 mm high, 21 mm inner diameter, 23 mm outer diameter, 10x23x23 mm.
  - Copied D2-R1 (D2-R2) and rotated it to degrees around X.
  - Created a cylinder (D2-R-ns) to clear some space inside the nuts where rings overlap, 50x11x11 mm.
  - Rotated D2-R-ns +90 degrees along X.
  - Moved D2-R-ns +1.5 mm Z. 
  - Created a cylinder (D2-ns1) to clear some space inside joint for ball to slide in, 3x20x20 mm.
  - Created a cylinder (D2-ns2) to remove unnecessary material under the joint, 3x20x20 mm.
  - Aligned All parts around X and Y.
  - Combined D2-R1, D2-R2, and D2-R-ns (D2-R).
  - Combined D2-M8n, D2-M8, D2-R (D2-F).
  - Combined D2-D1-ns, D2-ns1, and D2-ns2 with D2-F.
  - Printed Part-D2.
- Part-D3
  - Copied a G-clamp (D3-G) from a downloaded project (http://www.thingiverse.com/thing:1673030 clamp_frame_long.stl).
  - Rotated D3-G +90 around X so it stands as the letter U.
  - Created a cylinder (D3-ns-A), 10x9x9 mm. 
  - Created a cylinder (D3-ns-B), 6.5x15x15 mm.
  - Aligned D3-ns-A and D3-ns-B around X, Y, 0 mm Z.
  - Combined D3-ns-A and D3-ns-B (D3-ns1) and made it negative space. 
  - Rotated D3-ns1 +180 degrees X.
  - Copied D3-ns1 two times (D3-ns2, D3-ns3).
  - Aligned D3-ns1, D3-ns2, D3-ns3, and D3-G along X, set all to minimum shared Y.
  - Moved D3-ns1 +40 mm X.
  - Moved D3-ns2 +11 mm X.
  - Combined D3-ns1, D3-ns2, and D3-G.
  - Rotated D3-G +90 degrees so the flat side is DOWN.
  - Set D3-G Z to 0 mm.
  - Aligned D3-ns3 and D3-G along X, set all to minimum shared Y.
  - Moved D3-ns1 +9 mm X.
  - Combined D3-ns3 and D3-G.
  - Rotated D3-G back to original position for printing.
  - Printed Part-D3.
  - Printed G-clamps other parts (screw and clamp protector).
  - Printed a M8 screw and a M8 nut from metric screws project.

### Conclusions, version 1

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
- Part-D
  - Had a lot of problems printing Part-D2, it would often come off the printing sheet (making the result useless). This could be partly due to low grip on the printing plate (even with a brim) and difficulty printing overhands such as the top of the part, right below the threads.
  - Having multiple prints due to error in printing there was an epiphany as the multiple parts can stack on top of each other, meaning multiple Part-D1 and Part-D2 could for a long limb. Although that was part of the larger plan it was not expected to be achieved with version 1 as it was mostly to get a feeling for ball joint size and securing mechanisms.

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

### Part-B-v2

Using Part-B v1 as starting point.

- Copied Part-B (Part-B-v2)
- Locked Part-B-v2 in place.
- Copied M8 nut (M8n-B) from metrics screws project.
- Aligned Part-B-v2 and M8n-B.
- Rotated M8n-B 90 degrees so hole aligns with Y axis.
- Moved M8n-B -14 mm Y, -2 mm X so the nut is exposed on the side (Remember to add support structures).
- Alined Part-B-v2 and M8n-B with the bottom of Part-B-v2, then moved M8n-B 1 mm up Z.
- Copied negative space of Part-B-v2 (Part-B-v2-negative), moved it -2 mm Y.
- Combined Part-B-v2-negative and M8n-B to hide nut inside cradle.
- Locked M8n-B in place.
- Created new hinge for screw with circle instead of hex nut.
  - Created cylinder (Part-B-H), set size to 8x8x3.5 mm.
  - Created negative space cylinder for screw (Part-B-H-negative) as 4.5x4.5x5 mm.
  - Aligned Part-B-H-negative and Part-B-H along middle of all axes.
  - Combined parts.
- Created negative space cylinder (Part-B-H-negative) for Part-A hinge, 8x8x20 mm.
- Aligned Part-B-v2, Part-B-H-negative and Part-B-H along middle X and Y axis, bottom of Z axis.
- Moved Part-B-H-negative and Part-B-H +14.5 mm along X.
- Combined Part-B-H-negative and Part-B-v2.
- Combined Part-B-H and Part-B-v2.
- Created a box (Part-B-H-gap), 6x3.5x1 mm to fill cap under Part-B-H.
- Aligned Part-B-v2 and Part-B-H-gap along middle X and Y axis, bottom of Z axis.
- Moved Part-B-H-gap +8 mm on X.
- Combined Part-B-H-gap and Part-B-v2.
- Printed Part-B-v2. 

### Part-A-v2

Using Part-A v1 as starting point.

- Copied Part-A (Part-A-v2)
- Locked Part-A-v2 in place.
- Replaced M4n-A2 and M4n-A3 with round hinged used in Part-B-v2, along with gap fillers.
- Rotated M4n-A1 last +80 degrees along Y (was 10 degrees, should now be 90).
- Rotated M4n-A1 -90 degrees along Z so the hexagonal nut point up and down with a flat face toward +/- Y and hole though +/- X. 
- Copied M4n-A1 (M4n-A1.1).
- Aligned M4n-A1 and M4n-A1.1 with middle of Part-A-v2, top Z.
- Aligned M4n-A1 with max Y of Part-A-v2.
- Aligned M4n-A1.1 with min Y of Part-A-v2.
- Moved each 5 mm out.
- Rotate both -20 degrees so they now face more into Part-B
- Moved both -5 mm X.
- Moved both 1 mm in.
- Mode negative space for screw head (not needed but just in case).
- Add sloped supporting material so the printing of these nuts is easier, same way as gap filler with hinges. 

### Part-C-v2

Using metric-screws project, created longer screws that can elevate Part-A-v2 from Part-B-x.

- Copied M4 screw head (Part-C-v2-M4-1).
- Copied extended threaded shaft without a head (Part-C-v2-M4-2).
- Adjusted size of Part-C-v2-M4-2, toggle relative adjustment, set diameter to 4.4 mm.
- Centered Part-C-v2-M4-1 and Part-C-v2-M4-2 along X and Y, bottom Z.
- Measured 14.5 mm and cut the remaining off Part-C-v2-M4-2.
- Set Z of Part-C-v2-M4-2 to 3 mm (there will be a 0.5 mm overlap with Part-C-v2-M4-1, but the shaft will be 14 mm).
- Combined Part-C-v2-M4-1 and Part-C-v2-M4-2 (Part-C-v2-M414-1).
- Copied Part-C-v2-M414-1 (Part-C-v2-M414-2).
- Printed Part-C-v2.
- Adjusted width of shaft and thread up to 4.5 mm (Part-C-v2.1).
- Printed Part-C-v2.1.
- Adjusted width of shaft and thread up to 4.7 mm (Part-C-v2.2).
- Printed Part-C-v2.2.

### Conclusions, version 2

- Part-A-v2, Part-B-v2 elevation
  - Rounded hinges instead of nuts worked much better than expected, no need to remove gap under for the middle hinge.
  - Hinges have less wriggle room meaning less slack and inaccuracy, could be reduced by 0.25 or less on each side of the middle hinge.
  - Elevation solution 
    - The two screws are able to elevate the parts, but often slip and are hard to reach.
    - Quick fix is drilling holes for the screws to sit in on Part-B-v2.
    - Solution 1: using a screw-gear with a quarter of a normal gear plate, but the tolerances and alignment can cause issues.
    - Solution 2: parallel screws on a pivot that aren't angled towards Part-B-v2, M4n on a pivot on the sides of Part-B-v2. 
- Part-C-v2
  - Screws had to be adjusted up more than usual, seems like it could be the issue of Part-A-v2s vertical M4n nuts, but usually printing nuts vertically means they have less clearance for screws.
# arduino-arm

A small arm controlled by an Arduino board and servos. 

Correction from the drawings: 1 segment has been removed due to the weight of the limb and the inability for servo 1 and 2 to move it.

## Arduino code

The electronics ofo this project is covered by [this](https://github.com/grdall/arduino-projects/tree/master/projects/arduino-arm) repository.

## Assembly

This is a list for the minimum requirements for what can be defined as an arm. This will have a base, 1 segment, and 1 hand. For longer arms, simply add more segments.
Note that this is specifically for SG92R servos and the horns are fitted for their size. Models like SG90 have slightly larger horn requirements.

Part list:
- 1 base (subject to change)
- 1 segment base
  - 1 base-segment-coupler
  - 1 main-gear-pin-set
  - 1 main-gear-cut-sg92r
  - 1 small-gear-sg92r
- 1 segment
  - 1 segment-a1
  - 1 segment-b1
  - 6 segment-pin
  - 2 main-gear-sg92r
  - 1 main-gear-pin-set
- 1 hand
  - 1 hand-segment-a1
  - 1 hand-segment-b1
  - 1 hand-segment-c1
  - 1 main-gear-sg92r
  - 4 segment pins
- 1 set of fingers
  - 1 finger-a1
  - 1 finger-b1
  - 2 small-gear-sg92r
  - 2 finger-plate
  - 2 finger-plate-clip

1. Prepare the base:
  1. Insert the set of gear pegs in the cut main gears and take them out. This will make it easier to assemble later.
  1. Insert the set of gear pegs in the square holes on top of segment, with about 2 mm sticking out.

1. Prepare the segment:
  1. Prepare the segment pins by inserting them an taking the out of segment-b1. This will make it easier to assemble later.
  1. Insert the pins and servo in hand-segment-a1.
  1. Attach the main gear to the servo.
  1. Insert the set of gear pegs in one of the main gears and take them out. This will make it easier to assemble later.
  1. Insert the set of gear pegs in the square holes on top of segment, with about 2 mm sticking out.
  1. Repeat this process for each segment you have.

1. Prepare the hand:
  1. Prepare the segment pins by inserting them an taking the out of hand-b1. This will make it easier to assemble later.
  1. Insert the pins and servo in hand-a1.
  1. Attach the main gear to the servo.
  1. Insert hand-c1 into the top of hand-a1 and hand-b1.

1. Prepare the set of fingers:
  1. Place the plates with the extrusions up.
  1. Insert a small gear in the middle large hole.
  1. Insert either finger in the other large hole, with the concave part of the finger towards the small gear.
  1. Repeat this for the other plate.
  1. Place the plates together, gears facing each other, but not overlapping. You may need to wriggle the gears and align the fingers so they are mirrored.
  1. With the plates together and you can see the extrusions of both plates touching each other, grab the two finger-plate-clips.
  1. With a knife or thin tool carefully thread the clips over the outside of both plates, on the convex part near the square holes but don't push the clips into the holes yet.
  1. Make sure the fingers mirrored on each side and there are no overlapping gears before you pop the clips into the holes on the plates.

1. Insert the pegs on segment in the holes in segment base.
1. Attach the cut main gear to the segment base, outside the peg you just attached, on the same side as the servo horn.
1. Repeat this process for each segment you have, using normal main gears and the top of the previous segment instead of the segment base.
1. Insert the pegs on hand-segment in the holes in the top of the segment.
1. Attach the main gear to the top of the segment, outside the peg you just attached, on the same side as the servo horn.
1. Insert the set of finger in hand-a1 and hand-b1, just like with hand-c1, and lock it in place with the last servo.
1. You might want to secure the servo in hand-c1 to the set of fingers with a rubber band or a length of string.
1. Wire it all up.
# General printing tests

Various tests for printing, useful tricks and hacks.

## Horizontal sphere/arch sinking

Printing sound objects vertically (round side down essentially) makes them sink together, whether it is cylinder or a hole. Testing what level of design changes is needed to correct this.

Created a baseline by three cubes and three negative space cylinders with baseline pegs for testing. Cylinders are 5, 10, 20 mm diameter, while cubes are 10, 15, 25 mm tall. Negative space cylinders are 1 mm up and 2 mm from left of cubes, cubes were then put together so the holes are 2 mm apart (by vertical lines).

| Id | Modification | Orientation of holes | 5mm WxH | 10mm WxH | 20mm WxH | Can baseline pegs pass though | Corrective measures | Comments |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| I | None, baseline | Vertical | 5x5+ | 10x10 | 20x20 | Yes | - | 5mm peg is a little loose in it's hole, 10mm and 20mm fits very nicely with the slightest of rubbing against the walls |
| II | None, baseline | Horizontal | 5x5- | 10x10- | 20x19.5 | No | - | 5mm and 10mm pegs barely fit, 20mm peg does not as there is some overhang/collapse. Slight collapse on 5mm and 10 mm, but not enough to prevent pegs. |
| III | Increased height of negative space cylinders by 10% upwards | Horizontal | 5x5.4 | 10x11 | 20x21.5? | Yes | Change adjustment of negative space from 10% to 2.5% UP ONLY. Keep original negative space for even bottom. | Adjustment do no need to be at the bottom of a hole, only at the top. Furthermore the overhang at top caved more in than with ID I. The roof has some spacing, maybe as much as 0.1mm. |
| IV | Make copy of negative space, increase height by 2.5% | Horizontal |  |  |  |  |  |  |
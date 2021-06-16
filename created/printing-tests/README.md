# General printing tests

Various tests for printing, useful tricks and hacks.

## Horizontal sphere/arch sinking

Printing sound objects vertically (round side down essentially) makes them sink together, whether it is cylinder or a hole. Testing what level of design changes is needed to correct this.

Created a baseline by three cubes and three negative space cylinders with baseline pegs for testing. Cylinders are 5, 10, 20 mm diameter, while cubes are 10, 15, 25 mm tall. Negative space cylinders are 1 mm up and 2 mm from left of cubes, cubes were then put together so the holes are 2 mm apart (by vertical lines).

| Modification | Orientation of holes | Can baseline pegs pass though | Comment | Corrective measures |
| --- | --- | --- | --- | --- |
| None, baseline | Vertical |  |  |  |
| None, baseline | Horizontal |  |  |  |
| Incense height of negative space cylinders by 10% | Horizontal |  |  |  |
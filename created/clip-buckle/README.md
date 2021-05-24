# Clip buckle

Modeled on a clip buckle I have ([UTX Flex Side squeeze tm M-SS-1](https://sturtstreetcellars.com/utx-flex-side-squeeze-m-ss-1/)) I want to recreate something that could work together.

### Physical measurements (mm)

#### A

| Exterior | Max | Min | Indent Max | Indent Min | Outdent Max | Outdent Min |
| --- | --- | --- | --- | --- | --- | --- |
| Height | 11.5 | 12 | | | | |
| Width | 33.5 | 32 | 1.7 | 1.6 | | |
| Length | 46 | | | | | |
| Wall | 2 | 1.5 | | | | |

Housing is 33.5 long, rest is for belt loop.
Two rails on roof and floor of interior, 26 long, 1 mm thick, 2.5 spacing between, interior is max 9 min 7; total height of 9 - spacing of 2.5 = 6.5 for both rails / 2 = 3.25 height for each rail, rounding down to 3.
There is a 9 mm gap from inner wall to rail face.
Front extrusions are max 16, min 12.5 long front side.
Back extrusions are max 6, min 3 long from back side.
Indent is max 21, min 12 long


#### TODO

- Test scanner software (from images)
  - Test 3DF Zephyr (Free)
    - Worked for a pretty small object, but only to get general shape, surface was very rough and the entire part had to be remade, scan result wasn't even that much help.
    - Max cap. at 50 images for free version, not enough for small parts
  - Test VisualSFM + Meshlab
    - Unlimited images
    - Live visualized reconstruction
    - Minimal and older UI
    - Struggles sometimes to generate ref. points, generate multiple sparse and dense until a decent result.
    - Struggles similarly to 3DF Zephyr (Free)
- Free 3D scanners from images always (2 programs above) recreated 3D parts with too may inaccuracies and missing details to the point where items has to be recreated from scratch. Might as well just take a couple of images for reference and skip the lengthy generation process. Does not seem feasible for 3D printing.
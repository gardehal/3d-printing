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

- TinkerCad SVG method:
  1. Take images of object to model. 
    1. Prepare the object and the background. You want high contrast without shadows so the object pops right out in the SVG.
    1. Capture the object from as many angles as you need, flat on, with as few distortions as possible. Top, front and one side is enough for simple symmetrical objects.
      - Images will be flat (maybe doesn't need to be but I don't know enough about SVG and Inkscape to filter channels with height based on light or colour), so it might be good to take images from different angles and stitch them together in TinkerCad.
  1. Import the images to [Inkscape](https://inkscape.org).
  1. Convert to SVG (based on [this](https://designbundles.net/design-school/how-to-convert-a-jpeg-to-svg-in-inkscape) guide)
    1. Select file. Resize if necessary.
    1. Select image and click Path -> Trace Bitmap
    1. Click run? and wait for tracing to complete
    1. Once tracing is complete, click and drag the SVG? away from the image.
    1. Delete or hide original image.
    1. Click image metadata?, resize, fit to object?
    1. Save as "Optimized SVG"
  1. Import SVG to TinkerCad
    1. Click "Import" top right.
    1. Select the SVG on your computer.
    1. Set size 10%.
    1. Click "Import".
  1. Adjust the imported object
    1. Remove shadows or unrelated mass.
    1. Adjust the object to the size your real life object is, if you import an SVG of a coin that is 20 mm across, adjust the shape so it becomes 20 mm across.
    1. These object seem to be very complex and takes a while to load, exporting the trimmed object as STL and importing it again helps a little if you've made a lot of adjustments. Otherwise you can make a mold:
      1. Making your object a "hole".
      1. Encase it a shape as the mold.
      1. Combine mold and hole.
      1. Make mold hole.
      1. Place a shape inside the mold parameters, this will be the cast.
      1. Combine cast and mold. Now you have a copy of your SVG object which takes slightly less time to load in and manipulate.
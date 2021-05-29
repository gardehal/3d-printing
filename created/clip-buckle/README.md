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

#### Scanning software

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
      - Flash is optional but probably helps.
  1. Import the images to [Inkscape](https://inkscape.org).
  1. Convert to SVG (based on [this](https://designbundles.net/design-school/how-to-convert-a-jpeg-to-svg-in-inkscape) guide)
    1. Select file. Resize if necessary.
    1. Select image and click Path -> Trace Bitmap
    1. Select single scan with "Brightness cutoff".
    1. Select single, click "Apply" and wait for tracing to complete
    1. Once tracing is complete, click and drag the image away from the SVG.
    1. Delete or hide original image.
    1. Optional: Cut out the parts that are not important. This will same some time importing to TinkerCad.
      1. Select "Create rectangles or squares" in the menu on the left side of document (hotkey R).
      1. Make a rectangle over the content you want to keep (use white fill in rectangle for best result).
      1. Select the pointer (hotkey S).
      1. Select SVG and rectangle.
      1. Click Object -> Mask -> Set
      1. Set margin to at least 100 in Document Properties mentioned in next step.
    1. Click File -> Document Properties
    1. Under "Custom size" section, expand "Resize page to content...", select the SVG, and press the "Resize page to drawing or selection" button (select SVG and press hotkey Ctrl + Shift + R).
    1. Save as "Optimized SVG"
  1. Import SVG to TinkerCad
    1. Click "Import" top right.
    1. Select the SVG on your computer.
    1. Set size to fit within TinkerCads parameters, e.g. 10%.
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
  1. Combine the different aspects. Not a definitive guide, but worked for clip-buckle
      1. Take image from top of buckle, go though the process above.
      1. Adjust image so it was symmetrical (missed a little on perspective).
      1. Set width, length, height to 33x44x12.
      1. Take image of side of buckle, go though the process above.
      1. Rotate +90 degrees around Y.
      1. Set width, length, height to 33x44x12.
      1. Make "mold" of top view because it had less volume and more details to remove. Not sure if it matter which perceptive becomes the mold.
      1. Combine mold of top view and object of side view.
      1. Use measurements and objects created before to hollow insides and make rails.
      1. Export as normal.

      
#### Review 

Using image + SVG + TinkerCad was tricky to find out, but created a functional clip buckle receiver. There are some small adjustments, like how the catch-mechanism tapers more inward for a more secure grip. The part that attaches to a loop of fabric or belt was too weak and snapped off with little force as well, this needs more support. This version did not include the bar which the belt loops around either.
All in all it functions exactly the same way as the original, with less structural integrity. I also found a less manual way of copying physical objects though SVGs in TinkerCad. Project was a success.
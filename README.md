# 3D Printing

A collection of 3D printing projects.

## Dictionary

- Globbing, blobbing - when print results in large spheres of filament where it shouldn't be, common when attempting to print in thin air.

## Programs and tools

- Designing
  - [TinkerCad](tinkercad.com/) for creating the 3D models to print.
  - [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/free-trial) for creating the 3D models to print.
  - Calipers (preferably digital) for measuring physical object to copy or measure printing errors. [Useful printed part](https://hackaday.com/2018/09/09/3d-printed-radius-gauge-just-add-calipers-and-a-wee-bit-of-math/) for finding the radius of round objects.

- Printing
  - [Prusa Slicer](https://www.prusa3d.com/prusaslicer/) for translating 3D object to GCODE which the printer uses for printing.
  - [Prusa I3 MK3S+](https://www.prusa3d.com/original-prusa-i3-mk3/) for printing.
  - Knife for whittling down flattened first few layers of rounded object, brims, remove supports, and trim off small globs. Also useful to shave off test-strip which Prusa puts down to clear the nossle before each print.
  - A small flat head screw driver for scraping off material without risking damaging it, poking holes where needed.
  - Needle-nosed plyers for grabbing small misprint parts and supports in tight spots.
  - Flashlight to better inspect parts of print sometimes blocked by light during print.

## General resources

- [Thingiverse](thingiverse.com/) for community made 3D models.
- [Prusaprinters](https://www.prusaprinters.org) for community made 3D models. 
- [Sketchfab](https://sketchfab.com) for community made 3D models. 
- [Stlfinder](https://www.stlfinder.com) to find community made 3D models.
- [3D printing handbook](https://help.prusa3d.com/en/article/3d-printing-handbooks_125045/) that came with printer, contains some useful information.
- [Simplify3d](https://www.simplify3d.com/support/print-quality-troubleshooting/) common problems.

## General design knowledge

- Copying physical objects
  - [TinkerCad SVG copy method](#TinkerCad-SVG-copy-method), using photos of objects to make silhouettes which can be combined to make a 3D object.
  - [3DF Zephyr Free](https://www.3dflow.net/3df-zephyr-free/) or similar programs that combines images to make 3D representation of what's on the images (works best for large items).
- Design pitfalls
  - Printing holes. When printing holes that run parallel to the X or Y axis, some slicers may add some extra material to the roof of the hole or when bridging, or simply may miscalculate and create ovals instead of perfect circles.
    - Consider if you need a precise fit, if not, you could always increase the hole size.
    - Edit the holes in your design to be ovals (increase the height).
  - Impossible walls. When designing, sometimes walls or borders turn out to be so thin the slicer realise the printer is not capable of creating walls that think. Example: Design of a threaded screw that has a wall 0.1 mm thick, but the printer nozzles thinnest allowed setting is 0.15 mm. The result is that the slicer will ignore this wall. May depend on slicer and settings, some slicers can adjust nozzles of printers.
    - Keep in mind the thickness of walls and objects. Some tricky shapes includes threads on a screw, combination of multiple "hole" objects interacting when combined at once, calculations which creates shapes. 
    - Check your slicers settings, turn on warnings when impossible walls are detected.
  - Overhangs. Printing shapes with overhang above a certain vector leads to material not being supported and blobbing occurs.
    - Never print flat roofs without support.
    - Ensure the transitions from vertical to horizontal overhands are gradual and supported, the more corners the better.
    - Keep in mind "Printing holes" mentioned earlier in this list.
  - Supports. Supports are used when printing shapes that defy gravity. Consider printing an H oriented as it is in text. If the gap between the vertical lines are too large, the overhang over the horizontal line will sag or loosen the print from the plate, resulting in a failed print. Adding support to the horizontal line will allow for an easier print.
    - Supports can be added when designing, in you design software. Some downloadable designs will include this and sometimes put it in the description. 
    - Making supports in the design should be avoided unless absolutely necessary.
    - Some slicers have functionality to add supports, like PrusaSlicer allows users to paint areas to support, demonstrated [here](https://help.prusa3d.com/en/article/paint-on-supports_168584/).
    - Note that adding supports requires material and will increase print times.
    - Support should come of very easily, but removing them can damage fragile parts. Using tools such as knives may also cause damage to the print.
- Printing direction
- Infill
- Filament to use
- Combining parts glue vs. mechanical locking mechanisms 

## General printing knowledge

- First layer issues
- Warping
- Supports
- Brim
- Layer adhesion 

## Strengths and weaknesses

- Strengths
  - Print-in-place
  - quick prototyping
  - Lots of material ranging from soft and bendy to firm and snappy
- Weaknesses
  - Slower mass production
  - Mostly plastics and resin based material
  - Weaker than structure due to layering

## TinkerCad SVG copy method

  1. Take images of object to model. 
    1. Prepare the object and the background. You want high contrast without shadows so the object pops right out in the SVG.
    1. Capture the object from as many angles as you need, flat on, with as few distortions as possible. Top, front and one side is enough for simple symmetrical objects.
      - Images will be flat (maybe doesn't need to be but I don't know enough about SVG and Inkscape to filter channels with height based on light or colour), so it might be good to take images from different angles and stitch them together in TinkerCad.
      - Flash is optional but helps for contrasts.
      - Use a darker background or use flash to cast shadows.
  1. Import the images to [Inkscape](https://inkscape.org).
  1. Convert to SVG (based on [this](https://designbundles.net/design-school/how-to-convert-a-jpeg-to-svg-in-inkscape) guide)
    1. Import and select image. Resize if necessary.
    1. Select image and click Path -> Trace Bitmap
    1. Select single scan with "Brightness cutoff".
    1. Select single scan, click "Apply" and wait for tracing to complete
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
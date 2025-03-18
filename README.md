# 3D Printing

A collection of 3D printing projects.

## Dictionary

- globbing, blobbing - when print results in large spheres of filament where it shouldn't be, common when attempting to print in thin air.
- shell - the outer perimeter of an enclosed object.
- print in place - the act of printing moving parts locked inside a bearing or hinge of another part. These parts are designed to not come apart unless the bearing or hinge is removed or destroyed.

## Programs and tools

- Designing
  - [TinkerCad](tinkercad.com/) for creating the 3D models to print.
  - [Autodesk Fusion 360](https://www.autodesk.com/products/fusion-360/free-trial) for creating the 3D models to print.
  - Calipers (preferably digital) for measuring physical object to copy or measure printing errors. [Useful printed part, Hackaday](https://hackaday.com/2018/09/09/3d-printed-radius-gauge-just-add-calipers-and-a-wee-bit-of-math/) for finding the radius of round objects.

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
- [3D printing handbook, Prusa3d](https://help.prusa3d.com/en/article/3d-printing-handbooks_125045/) that came with printer, contains some useful information.
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
    - Some advanced prints don't need support, while seemingly simple prints needs lots. Spotting what needs support comes with experience, or tools like PrusaSlicer can detect areas at risk (see demonstration of PrusaSlicers paint on support tool).
    - In the end, it's better to add 30 minutes of support making to an 8 hour print than it is for the print to fail 7 hours in and having to start over.
    - Note that infill can stick really well to the print and be very difficult to remove, or that you may damage the print in the process of removing supports.
- Printing direction. The orientation fo your model in the slicer will determine the printing direction. 
  - General rule of thumb is that a print will be the weakest where layers interact with indents or cutouts.
  - Consider printing the letter L, orientated as written. A printer that prints from the bottom up will create an L with a string horizontal like but weak vertical line, even if they are identical in the design. This is because the layers will run parallel the horizontal line. Attempting to snap the horizontal line will be like attempting to snap a bundle of sticks. The vertical line is also layered the same way, and breaking it is like snapping a coin roll in half.
  - Whenever strength is needed for a part, print it in such a way that the bending force is applied perpendicular on the print lines.
  - Printing direction may also affect parts fitting. Although two parts fit together in theory, and even when printed one way, they may not fit if one or both are printed another way.
- Infill. The filament added inside the shell.
  - Infill percentage is often used to determine how much of the internal volume will be filled, ranging from 0% to 100%.
  - There are different patterns available for infill, some are stronger, some are faster, and some of more economical.
- Picking filament. Filaments made from different material have different properties.
  - Filament of different types often require different temperatures.
  - Some filaments are notorious for printing errors and difficulties printing, eg. nylon, some PETG types.
  - Pick a filament that is best suited for your usage. PLA is best for small indoor items like trinkets and semi-flexible parts, better for the environment. PETG is stronger and more rigid, resist weathering better, easier to sandpaper down.
  - There are various filaments that mocks the feeling and appearance of non-filament. An example is wood filament, which contains some thermal resin or plastic like PLA and sawdust.
- Combining parts. Projects sometimes call for multiple parts because they are too complex to print as one, or is intended to move, lock, or transform.
  - Locking mechanisms, some cases and uses:
    1. screws, threaded nuts and bolts. Useful for moving varying degrees of pressure. Also lots of options, as long as the threads are not build into the design, separate nuts and bolts can be printed, or metal ones can be used for a fixing less likely to break than your print.
    1. pegs, anything from simple rods, spring loaded (akin to a LEGO "Technic Peg with Friction" or the pin used in chair-rail-mount) to complex keys. Useful for contraptions with some tension to keep them in place, or as temporary fasteners that is intended to be set up and taken down by hand. Pegs with a spring loaded latch can be especially useful as they secure in place without falling out, but can be removed by hand.
    1. tapering/friction, such as telescoping. Mostly used for projects that call for some growing and retracting, like a old school extendable telescope. Due to weakness of plastics and resins.
    1. clamps/snap-in, such as snap buckles or other hooks with slots. Can be used for prints that require parts to snap in place in a specific way, can be made such that it's very hard to undo without damaging the parts, or an opening around the hook so it may be undone.
  - Print-in-place, some cases and uses:
    1. smaller objects, fewer prints, harder to repair, overall quicker.
  - Glue, works best for:
    1. rough surfaces, for example sanded down or perpendicular to print lines.
    1. small parts that cannot use any method mentioned above (or in combination).
  - Other temporary, non-printed, easily reversible methods:
    1. magnets, nice for parts that conveniently open and close with some elegance. Mind the damage it may do to data storage or computers. 
    1. string, for a more esoteric or mystic theme, also common and cheap.
    1. velcro, can be used for parts that doesn't need to be exact, but rather simple  and quick.
- Big/Complex models can be simplified loading it into Autodesks MeshMixer -> Cut/Edit as needed -> Export .stl -> Load into slicer with a repair/fix function (e.g. Prusa Slicer) -> Load into whatever program had a size limit

## General printing knowledge

- First layer issues, the first layer tends to have various issues, which can depend on printer settings and sloppy design. For my Prusa MK3, these issues include:
  - Nozzle being too far away from bed, causing filament to come loose and blob.
  - Nozzle being too close to the bed, extruding too much filament and causing excess filament to create blobs 
  - Round objects being deformed with a flat area towards the bed.
  - Difficulty removing print due to first layer being stuck.
  - Best fixes is to do test prints with different Z offset-settings, checking all prints before 5th layer, issues with first few layers are usually obvious by then.
- Warping, causing prints to warp, adding curves to parts that are expected to be straight.
  - Unknown why it happens, possible due to heating differences
- Printers and prints oscillating, if the printer bed moves, can cause tall prints to move or come loose which ruins the print. Printers with large amount of moving parts can also cause the entire printer to move.
  - For printers with movable beds, use a brim to better grip the bed.
  - For printers with movable beds and where brims are nor working, orientate the print some other way. With supports it's possible to print long shapes diagonally.
  - Printers with large moving parts should be placed in some material that cushion and absorbs the movement. Building or furniture foam under a heavy, stiff base like a slab of concrete or rock should work. See [this video](https://youtu.be/y08v6PY_7ak) for more details.
- Brim, first layer added material around the base of the print.
  - Brims can be useful to secure small items to the bed and prevent blobbing.
  - Are sometimes hard to remove, or removing them can damage the print.
- Layer adhesion, how strong printed layers stick together. Adhesion is improved when:
  - The extruder is forcing filament onto the previous layer, either by setting the height of each layer, or by increasing the speed or volume filament is fed though  the nozzle.
  - The previous layer is heated so the filament binds better.
  - Dust and particles in the room is kept to a minimum.

## Strengths and weaknesses

- Strengths
  - Print-in-place - a technique which enables printing parts captive inside others, eliminating the need for adding complex connection devices and allow moving pieces to be smaller.
  - Quick prototyping - no need to spend hours creating wooden or metal shapes, or even mold for plastics.
  - Lots of material - ranging from soft and bendy to firm and snappy. 
- Weaknesses
  - Slower mass production - not suited to create large volumes of products.
  - Mostly plastics and resin based material - limiting materials that can be used, but there are metal 3D printers which are very expensive.
  - Weaker structure - weaker than some other plastic production due to printing layering thin strings of filament at a time, allowing for plastic not to bond properly.

## TinkerCad SVG copy method

  1. Take images of object to model. 
    1. Prepare the object and the background. You want high contrast without shadows so the object pops right out in the SVG.
    1. Capture the object from as many angles as you need, flat on, with as few distortions as possible. Top, front and one side is enough for simple symmetrical objects.
      - Images will be flat (maybe doesn't need to be but I don't know enough about SVG and Inkscape to filter channels with height based on light or colour), so it might be good to take images from different angles and stitch them together in TinkerCad.
      - Flash is optional but helps for contrasts.
      - Use a darker background or use flash to cast shadows.
  1. Import the images to [Inkscape](https://inkscape.org).
  1. Convert to SVG (based on [DesignBundles](https://designbundles.net/design-school/how-to-convert-a-jpeg-to-svg-in-inkscape) guide)
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
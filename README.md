# 3D Printing

A collection of 3D printing projects.

## Programs and tools

- Designing
  - TinkerCad

- Printing
  - Prusa MK3..

## General resources

## General design knowledge

1. Copying physical objects
1. Find relative stretch needed to make perfect horizontally printed holes
1. Design pitfalls
1. Pitfalls with screw threads and "impossible walls" 
1. Overhangs 
1. Printing direction
1. Infill
1. Filament to use
1. Combining parts glue vs. mechanical locking mechanisms 

## General printing knowledge

1. First layer issues
1. Warping
1. Supports
1. Brim
1. Layer adhesion 

## Strengths and weaknesses

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
# 3D Printing Nuts and bolts

## Metric Bolt Sizes
Metric nuts and bolts are commonly referenced using ‘M’ sizes, for example: M3, M8, M12. But the size of a metric fastener is more accurately specified using diameter, pitch and length dimensions, in millimeters. For nuts the size dimensions used are simply diameter and pitch.

Here’s an example metric bolt specification: M8-1.0 x 20

This bolt specification breaks down like this:

The letter ‘M’ indicates that this bolt uses a metric thread.
The number ‘8’ refers to the nominal diameter of the bolt shaft in millimeters.
The number 1.0 is the thread pitch of the bolt, which is the distance between threads, in millimeters.
And the final figure, 20, is the length in millimeters.
But it’s very common to see metric bolts specified like this: M12-50.

This abbreviated format omits the pitch definition which means that the bolt has a coarse thread. Whenever the pitch dimension is omitted from a metric bolt specification then the bolt is always coarse threaded. This example (M12-50) has a diameter of 12mm and a length of 50mm.

Source: https://www.insight-security.com/get-to-know-metric-bolt-sizes

## Standard Spanner and Allen Key Sizes

| Size | Spanner | Allen Key |
| --- | --- | --- |
| M2 | 4 mm | 2 mm |
| M3 | 5 mm | 2.5 mm |
| M4 | 7 mm | 3 mm |
| M5 | 8 mm | 4 mm |
| M6 | 10 mm | 5 mm |
| M8 | 13 mm | 6 mm |
| M10 | 17 mm | 8 mm |
| M12 | 19 mm | 10 mm |
| M16 | 24 mm | 14 mm |
| M20 | 30 mm | 17 mm |
| M24 | 36 mm | 19 mm |
| M30 | 46 mm | N/A |

Source: https://www.insight-security.com/get-to-know-metric-bolt-sizes , https://www.polymax.co.uk/metric_spanner_sizes , https://www.sailsetc2.com/index.php/products-by-category/fittings/tools/allen-key-alone.html

## Hole Sizes for Metric Bolts

| Size | Clearance Hole mm | Thread Pitch (std) | Tapping Drill (std Pitch) | Thread Pitch (fine) | Tapping Drill (fine pitch) |
| --- | --- | --- | --- | --- | --- |
| M2 | N/A | N/A | N/A | N/A | N/A |
| M3 | N/A | N/A | N/A | N/A | N/A |
| M4 | N/A | N/A | N/A | N/A | N/A |
| M5 | 5.5 | 0.8 | 4.2 mm | N/A | N/A |
| M6 | 6.5 | 1.0 | 5.0 mm | 0.75 | 5.25 mm |
| M8 | 9 | 1.25 | 6.75 mm | 1.0 | 7 mm |
| M10 | 11 | 1.5 | 8.5 mm | 1.0 or 1.25 | 9.0 or 8.75 mm |
| M12 | 14 | 1.75 | 10.25 mm | 1.5 | 10.5 mm |
| M16 | 18 | 2.0 | 14 mm | 1.5 | 16.5 mm |
| M20 | 22 | 2.5 | 17.5 mm | 1.5 | 20.5 mm |
| M24 | 26 | 3.0 | 21 mm | 2.0 | 22 mm |
| M30 | 32 | 3.5 | 26.5 mm | 2.0 | 28 mm |

Source: https://www.insight-security.com/get-to-know-metric-bolt-sizes

## Printing tests

Testing using Prusa mk3i with Prusa Slicer and TinkerCad web. 0.05 tip, 20% infill, PLA.

Y correction 1.300:

- M3 - FAIL
  - Nut and bolts are too coarse to be used together. 
  - Nut is very difficult to use with metal M3 but it works. 
  - Screw with metal nut works but is hard to start.

- M4 (marked "I") - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.

- M5 - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.

- M6 - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.

- M8 (marked "I") - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.
  - Bolts and screws are 8 mm with threads.
  - Inner nut with threads is 6 mm.
  - One side of a screws threads are flat, the other is sharp.
  - Bolt is mostly flat.
  - PLA strings on screw seems to be on flat side, but bolts sharp threads are close to strings.
  - Maybe only printing one screw helps with flat threads.
  
  Conclusions:
  - Screws and bolts threads are flat, they do not work with their respective nuts.
  - Nuts seem to have good threads.
  - Some screws and bolts work with larger nuts, so far best one is M5 screw with M6 nut, smooth action, cannot pull off with just hands.
  - Layer adhesion seems good.

Y correction 1.250:

- M4 (marked "II") - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.
  - Nut bottom messed up a bit.
  - Threads SEEM LESS flat than M3 I.
  - Layer adhesion seems good.

Y correction 1.350:

- M4 (marked "III") - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.
  - Threads SEEM MORE flat than M3 I.
  - Layer adhesion seems good but looks more is squished with small blobs

Y correction 1.200:

- M4 (marked "IIII") - FAIL
  - Nut and bolts are too coarse to be used together. 
  - No metal bolts or nuts to test with.
  - Nut bottom messed up a bit.
  - Threads SEEM MORE flat than M3 I.
  - Layer adhesion seems good.

- Conclusions:
  - Y level 1.250 - 1.300 seems optimal.
  - Threads are flat regardless of Y level. Testing different designs...

Y correction 1.300, testing new design:

- M8 ? M7 - SUCCESS
  - Different design.
  - Was uncleanly marked, turns out to be 7 mm across the threads.
  - Advertized as M8.
  - Bolt head 1 mm smaller than M8 head.
  - Bolt head 1 mm larger than M6 head.
  - Nut is a bit loose, wriggles around shaft whe not tightened (less than 0.5 mm between nut and bolt).
  - Nut can be wriggled 1 mm up the shaft from lowest point to highest point.
  - Threads are larger than previous design.

- Conclusions:
  - Seems like previous designs, assuming that is the correct Mx screws, are too fine threaded to be printed.
  - Ideally the real world Mx screws would be used, so printed parts can be changed with metal parts without any fuzz.
  - New design is more printer friendly.
  - Test new design scaled up to M8 and down to M6 and M4.
  - Test new design extruder minimum size.
  - Old Mx designs can be used to cut out paths where metal parts are needed, although these parts don't really need grooves, so an M3 screw only needs a 3 mm hole and maybe a negative space for the nut.

- M8 (marked "II") - SUCCESS
  - Corrected M8 ? M7 up ONE mm (bolt head flats) from 12 (head) x 13.86 (head) x 30 (tall) to 13 (head) x 15.02 (head) x 32.50 (tall)
  - Same design mas M7 ? M8.
  - 8 mm across the threads.
  - Bolt head is the same size as old M8 design head.
  - Bolt head 1 mm larger than M7 ? M8 head.
  - Nut is a bit loose, wriggles around shaft whe not tightened (less than 0.5 mm between nut and bolt).
  - Nut can be wriggled 0.5 mm up the shaft from lowest point to highest point.
  - Nut wriggles less than M7 ? M8.

- M4 (marked "IV") - SUCCESS
  - Corrected M8 II down to 7 (head) x ? (head) x ? (tall).
  - Nut wriggles very little.
  - Too much resistance to spin freely.


Testing using Prusa mk3i with Prusa Slicer and TinkerCad web. 0.15 tip, 15% infill, PLA.

- M8 (marked "III") - Bolt SUCCESS, nut FAIL
  - MORE details on threads than M8 II.
  - Printing time reduced more than 3 times.
  - Bolt was printed with some loose threads, nut failed 1/4th of the way in.
  - M8 II bolt wriggles more on M8 III than on M8 II bolts.
  - Can be broken with bare hands.

Testing using Prusa mk3i with Prusa Slicer and TinkerCad web. 0.20 tip, 15% infill, PLA.

- M8 (marked "IV") - SUCCESS
  - Slightly less details on threads than M8 III.
  - Plastic strings are larger than 0.15, unsure what is preferable.
  - Can be broken with bare hands.

- M4 (marked "V") - SUCCESS
  - Better detail threads than previous M4 screws.

Testing using Prusa mk3i with Prusa Slicer and TinkerCad web. 0.15 tip, 25% infill, PLA.

- M8 nut (marked "V") - FAIL
  - Attempted to shrink inside of nut with 0.25 mm by putting a smaller nut inside the existing M8 nut.
  - Nut still fits 8 mm M8 screw but also rattles, though significantly less.

- M8 (marked "VI") - FAIL
  - Attempted to shrink inside of nut with 0.5 mm by putting a smaller nut inside the existing M8 nut.
  - Nut rattles more than M8 V nut.

- M8 nut (marked "VII") - FAIL
  - Negative space hexagon with screw.
  - Threads too fine in nut.

- Conclusions:
  - 0.15 mm tip seems like a good all-around size.
  - 0.20 mm and larger for faster builds, prototypes.
  - 0.10 mm and smaller for detailed builds ONLY when 0.15 mm fails.
  - 20% infill with 0.05 mm tip is pretty strong (relative to other bolts, se point below).
  - 15% infill with 0.15 mm and 0.20 mm tip relatively weak.
  - 20% infill should be base infill level.
  - ALWAYS use brim, screws have always failed when it's off.

- M8 nut (marked "VIII") - SUCCESS
  - Attempted to shrink height of nut with 1.00 mm by putting a smaller nut inside the existing M8 nut. Center all axes.
  - Almost perfect fit for a M8 VI bolt.
  - Nut no longer spins freely if flicked.
  - Very little wriggle up down, still some left right.
  - 1 mm larger (14 mm) than the M8 VI bolt head (13 mm).
  
- M8 nut (marked "IX") - SUCCESS
  - Attempted to shrink height of nut with 1.00 mm by putting a smaller nut inside the existing M8 nut. Center all axes.
  - Checked sized before merging parts, should be standards M8 size (13 mm).
  - Same benefits as M8 VIII, but the correct size.

- M8 (marked "X") - FAIL
  - Printed a set of the rounded screw heads.
  - Shaft with threads is around 8.5 to 9 mm, does not even fit with the loose nuts.
  - Probability of need to be redesigned.

- M8 (marked "XI") - FAIL
  - Scaled screw down 1 mm.
  - Nuts now fit, but rattle too much.
  - Redesign is necessary.

- M8 (marked "XII") - FAIL
  - Remade all M8 screws to an uniform 5.5 mm tall head, 15 mm at the widest, 13 mm on the hex flats.
  - Remade all M8 screws to 30 mm tall (long).
  - Threads turned out 7.5 mm.
  - From the printing layers it seems that adjusting the Y correction slightly could yield one more line 
  - Head is 13 x 14.9 - 15 mm x 5.5 mm.
  - Screw is 30 mm long.
  - Design program and encoding program says 8 mm.
  - Unsure if error is in design program, transfer from design program to printer encoding program, encoding program, or print.

- M8 (marked "XIII") - INCONCLUSIVE
  - Adjusted one bolt-object 0.5 mm for assumed printer error.
  - Measures out exactly 8 mm.
  - M8 IX nut rattles more than it does on < IX bolts.
  - Adjusted one bolt-object 1 mm for assumed printer error.
  - M8 + 1 mm too large, came out as 8.5 to 8.75 mm.

- M8 (marked "XIV") - SUCCESS
  - Adjusted one bolt-object 0.75 mm for assumed printer error.
  - Design measurements head: 13x15x5.5 mm
  - Design measurements shaft: 8.75x8.75x24.5 mm
  - Physical measurements head: 13x15x5.75 mm
  - Physical measurements shaft: 8x8x24.5 mm
  - M8 VIII nut fits very well, minor rattle.
  - M8 IX nut fits perfectly, almost no rattle.

- M8 (marked "XV") - SUCCESS
  - Printed 1 bolt and 1 nut 
  - Design measurements nut: 13x15x6.5 mm
  - Design measurements head: 13x15x6.5 mm
  - Design measurements shaft: 8.75x8.75x24.5 mm
  - Physical measurements nut: 13x15x6.5 mm
  - Physical measurements head: 13x15x6.5 mm
  - Physical measurements shaft: 8x8x24.5 mm
  - M8 XV nut fits very well, minor rattle.

- M4 (marked "XV") - FAIL
  - Printed 1 bolt and 1 nut 
  - Nut and bolt does not fit together at all, screw clears hole.
  - Nut is too tight for M4 IV bolt.
  - Screw is too thin for M4 IV nut.

tdoo
  - Design measurements nut: 13x15x6.5 mm
  - Design measurements head: 13x15x6.5 mm
  - Design measurements shaft: 8.75x8.75x24.5 mm
  - Physical measurements nut: 13x15x6.5 mm
  - Physical measurements head: 13x15x6.5 mm
  - Physical measurements shaft: 8x8x24.5 mm



  - Screw shaft with threads is about 3.5 mm, should be 4 mm.
  - Allen key slot is barely 2.5 mm but a 2.5 mm allen key doesn't work. 
  - 3 mm allen key with chamfering can be forced into slot and will turn the screw.
  - Will reprint with + 0.75 mm.   

# Volumetric Colony Counting

A standard means of detecting the presence of bacteria is "plating". A growth medium, often a gel made with agar, is inocculated
with potential bacteria. After a certain time, the bacteria forms colonies. If the bacteria creates a by-produt 
which makes a colorimetric change to a dye, perhaps based on pH or the production of a gas, the "colony" may be visible to the
naked eye, though the bacteria themselves are often not visible. Generally bacteria are so small they are barely visible 
or not visible under the highest optical magnification.

This process is often an "area based" process. That is, the medium is thin, on a "plate" or a "film". The material
which is testable is therefore proportional to the area employed.

In the case of water testing, it is common to wish to test 100 ml of water. Some plating (Petrifilms) allow only 1 ml 
per plate. Some allow up to 5 ml per plate.

When a larger volume is required, membrane filtration can be used to increase the concentration of the bacteria 
in the sample. This requires some careful handling, but increase the effective sample size per plate.

## Idea: use a volume rather than an area

If we could instead grow colonies inside a medium, we could directly test a large sample within a smaller linear space.
However, it may not be possible to see the colonies within a block of growing medium.

Imagine a cube of growth medium, containing colonies inside it, possible marked by dyes. 
It may be possible by moving the focal plane through the cube to focus on individual slices of the growth medium.
In this way, changing the position and focus of a microscope, we might be able to automatically detect colonies 
in a volume. This could be extremely efficient.

This has been made much easier to study based on recent open source microscopes such as the [FlyPi](https://github.com/amchagas/Flypi).

Since the volume of the dye associated with a colony may exist in multiple focal planes, this is a good candidate for
algorithmic computer vision-based detection of the colony.

Alternatively, we might be able to create a spiral which can be unwound to use traditional view mechanisms on a volume.
This would be similar to the way an old-style film canister works. A coil of a strong strubstrate bonded to a growing 
medium could be used. However, this mechanically more complicated.

If the medium is not optically clear of if the the growth of colonies produces sufficient occlusions, it may be difficult to
identify colonies due to occlusions.

## Impact: huge, in some cases

This approach might allow us to potentially identify colonies in larger samples. If this is simpler than membrane filtration,
or for bacteria which are difficult to isolate via membrane filtration, it seems that this approach could significantly
improve important subsets of basic bacteriology.

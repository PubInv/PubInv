# Motile Ferrofluid Snail/Slug

Imagine a little device like a slug that could move inside a sea of ferrfluid like a little fish or submarine. It would be very cool if this
device could move without any moving parts whatsover. If we had such a device, we could put it in a tube and have a pump---if the slug
can swim forward, it must push the ferrofluid backeward.

Imainge a pair of coils, about 1 cm in dimater, separated by about 0.5 cm. Imagine then with current flowing in the same direction,
but controllable in the sense that the current to one or the other maybe be doubled.

Now imagine 5 pairs of such coils with their axes vertical arranged horizontally, a little like (IIIII). Now if this
is immersed in ferrofluid and sufficiently energized it will be covered in ferrofluid, even against the force of 
gravity.

Imagine now that one moves the greater current in a circular pattern. That is, imagine the top coil of each pair
receiving greater current in turn, so that a lump of ferrofluid is carried to one end. Then at the end the bottom coils is 
maximally energized, moving the lump to the bottom.  The wave then moves in the opposite direction along the bottom,
until the process repeats.  This entire assembly will potentially move on the basis of the anisotropic flow along the bottom.

This would only take about 2 days to test out.  Potentially the frame would have to be constructed to hold the coils and
the coils would have to be wound. An arduino program in combination with a motor shield with 10 channels would have to be 
created to control the addtional voltage (or possibly relays, or a transistor, or a multiplexer could be used.)

## Tremendous Progress -- A Passive Ferrofluid Valve

Veronica Stuckey and I have submitted [this paper](https://github.com/PubInv/ferrofluidcheckvalve/blob/master/doc/SmartMaterials/ioplatexguidelines-1/FerrofluidCheckValve.pdf) to Smart Materials. It describes one of Public Invention's best inventions: a passive ferrofluid check valved.

I belive it may be possible to use a similar idea to make a solidstate pump by using a shaped chamber and an oscillating magentic field.
The basic idea is that in an assymetric 2D chamber, a strong magnetic field will attempt to draw fluid into the center of the field. 
If the opening on one side accesses more fluid than on the other, it will create a force to squeeze the fluid into the narrower side.
When the field is relaxed, there is no force for it to return. The result is that by simply oscilatting the field, we can make a true
pump for ferrofluid which has no moving parts.

![Idea for Pump](https://user-images.githubusercontent.com/5296671/146234698-07b2f31f-3cca-459b-bb94-ae29e1e219d2.png)


## A Frequency-based Ferrofluid Pump - Nov. 2021

This problem is almost the same as making a Ferrofluid Pump with either no moving parts or minimum moving parts.
Based on our work on a [ferrofluid check valve](https://github.com/PubInv/ferrofluidcheckvalve), we now believe this 
may be more possible than we originally imagined.

A solid-state pump would be extremely valuable as something that could be made "on-a-chip". This micro-scale 
application would allow fluid manipulation on a very small scale.

The basic idea that there may be frequency-effects on ferrofluid does not seem to have been written about much.
That is, ferrofluid in a rapidly oscillating magnetic field may behave in interesting ways that allow magic
things to be done. The iron nanonparticles within ferrofluid align themselves quickly with a magnetic field,
but not instantaneously. A magnetic field modified on the time scale of this alignment could create unique
situations. For example, there might be a certain feqrency at which two varying coils could create an assymetric 
force on the fluid. If two or more simple coils around a pipe filled with ferrofluid could drive the fluid
in one direction based on high-freqnecy oscillation, it would be quite an acheivement.
It is possible this is not possible in a simple tube, but may be possible in combination with an assymetric
geometric, as we have successfully shown in the [ferrofluid check valve](https://github.com/PubInv/ferrofluidcheckvalve).

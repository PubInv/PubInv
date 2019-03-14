# Status: Closed in favor of Project #45

This project spawned [Project #45](https://github.com/PubInv/segmented-helixes), which is highly active. This project is closed in favor of that project.

# Concept

It is a fact, perhaps surprising, that if you take any object and make an unbounded number of copies of it and always place
a second copy in the same orientation to a first copy, the resulting collection of objects is essentially a helix.

This fact was "discoverd" during the Mathathon, and confirmed by a paper and private communication with Dr. Eric Lord.
I have in fact since that time worked out a Mathematica program that computes the radious and pitch of the helix based on only
the intrinsic properties of the object joints.

# The Problem

It would be nice of the function of for the radius of this helix was given by a nice close-form expression of the length of
the object and the angular relationship. In fact, there is a such a formula, but it has about 50 terms. It is beyond human
comprehension.

There are, however, ways we can still make use of this formula. For example, we graph special cases. Better yet, we 
can make software that allows you to enter the angular displacement and automatically computes (and renders in 3D) the 
object stacking the conincident helix induced by it.

The project is to produce such a tool in a browser deliverable for in Javascript.

# Skill required

Because the mathathon has already produced a good bit of similar software in Three.js, this project need not start from scratch.
I recommend we take this software and modify it specifcically for this purpose. The rendering of the objects is 
essentially already done.

The linear algebra will of course have to be translated from Mathematica to JavaScript, but that would be relatively simple.

Finally, a certain amount of user interface work would have to be done to make it usable.

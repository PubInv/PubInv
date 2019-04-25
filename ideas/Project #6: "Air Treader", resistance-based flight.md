# Initial design for a tiny table-top prototype

Here's a very basic design for a buildable version of an air-treader that could begin research.

The basic idea is to develop a form of "flight", or perhaps "falling with style", that is slower and safer than normal flight.
Propellers are actually about 90% efficient, so it may not be possible to beat that.  However, it may be possible 
to develop a mechanism for flight, or at least levitation, based on principles other than the air-foil based propeller.


# Series Drogue

Mariners use a device called a drogue.  it is similar to a parachute.

We can posit the following mathematical question:

What is the shape that produces the highest possible drag that can fit within a cylinder of a certain size?

We posit that if the cylinder is long enough, two parachutes will have a higher drag than one.

But suppose the cylinder has an aspect ratio of 4 to 1?

How much would a 4-chute system have higher drag than 1-chute system?  And, in a 4-chute system, is the standard parachute shape really best?  Perhaps something which allows more flow is actually better?  Perhaps even something that produces some horrible vortex or something?  Perhaps a certain amount of flow is required to get the advantages.

Can we in this way build an “air drogue” that would allow resistance-based flight more effectively?


http://flowsquare.com

Looks like this can be used as a simple way to answer the multiple-chute question.

We might even be able to answer the question of what kind of force we can exert this way!

The basic idea is to have drogue-on-a-pole.  You ram the pole upward, then you pull down on it.  The drogue is higly directional in drag, so you exert a directional force.  For balance, you could make this like a quad-copter.

The result could be more efficient flight --- or perhaps, more efficient-levitation would be a better way of thinking about it.

Note it is possibly that a series drogue in Air should have the first chute be small so that the air spills into the second, etc.

It is possible also that the first chute should be a ribbon chute, and that the porosity should reduce to zero by the final chute.  Perhaps this can create maximum turbulence, and therefore drag.  Or possibly we want a system that ejects air in streams in different directions to create maximum drag.  This is a good problem because it combines physics, computation, and other practical concerns.

For example, what if the first for chutes were scoops, shaped like Elbow Macaroni, that ejected air in four directions as broadly as possible!  Then the turbulence would be maximized!  This is mathematically interesting --- or what if if it even blow the air back down!  An air muffler!

Obviously, conservation of energy applies --- but still.  What if you build a shape that forces 90% of the air downward?  Simplest answer: in outer ring forces air back under to the center of the chute.  Like a hovercraft.



Question:  If you build a toroidal parachute, won’t the air natural circulate from inside to outside anyway?

Note toroidal chutes may already exist:

https://www.fruitychutes.com/parachute_recovery_products/iris_ultra_parachutes.htm

As far ast I can tell, the internal circulation idea does not work.

Idea: Can we actively PREVENT vortex shedding in order to create a higher-drag environment?

Ideas:

Create this with carbon fiber arrow shafts using a solenoid, rather than a rotational motor.  Could constuct a model with a single shaft, the whole thing would be very narrow.

Idea:

Make the thing like a sea slug: a tube, in which the drogues are on lines that run up the middle of the shaft and outside.  The machine pulls the lines around, and at the bottom the drogue collapses and is pulled back up the middle of the tube, to come out the top again and open at that point.  This would be a smooth, continuous flow, rather than a jerky motion.

Could still use a solenoid concept to smoothly pull the lines.  Might be able to use pre-manufactured chutes in this case.



There is some argument that long solenoids are a little tricky:

http://electronics.stackexchange.com/questions/28878/long-solenoid-50cm-stroke

But I am sure it is a solvable problem one way or another.

Idea:  Create a linear vertical air pump -- a “Drogue pump”.

Have a series of cones on a pole.  Have some mechanism for moving the cones back and forth, which will directionally pump air out in the downward direction.  However, at the same time you will be using the resistance mechanism to stay aloft.  if you quite pumping, you just fall down.


Experiment:

By 3 cheap umbrellas, and drop from a tree to time the fall.

Compare this to a one-umbrella configuration.

Some basic problems:

How do you build light, long, actuator?  Possibly build my own pneumatic cylinder?  Drive this with hydraulics and solenoid?

Or build a coil gun?

How do I get carbon-fiber rods?

Where do I get rip-stop nylon?  Nylon thread?

New Idea:

You build a tower with 3 or 4 or 6 heads, and each head is a pulley, and you make running drogue line over this. Sadly you now have a beam-problem.  In the base you have a simple circular motor that is pulling all lines around.



In this system, we have to have a reliable way to close the chutes --- potentially a problem, but perhaps it acts as an “air pump” anyway.

So this translates simple motion, and there are always chutes open, so hopefully it is very safe.  We of course have some structural engineering problems, and some other problems, but in principle this could be far more efficient than wing-based flight, and take up less space.

How do you get a chute to close rapidly while it is moving?

However, I now believe a telescoping pole is a far simpler solution.  I believe this could be made as a pneumatic cylinder.  However. possibly it could be made with a “mirror mechanism” as well.

Here is a small challenge: 
Build a machine that:
hovers,
falls gently to earth if the power is cut under all circumstances,
fits into a box 12” in a side when not in flight without any assembly or disassembly, and
uses less power than a quadcopter to hover the same mass.

Note:

An additional idea is to build a “drogue fabric” --- maybe create 100 drogues.  Note that although difficult to manufacture, the challenge of creating a very small drogue out is rather intersting.  We can imagine a solenoid pushing on an air-hydraulic system, which drives a very thin rod up and down at magnified linear extent.  This is actually a very interesting approach on its own --- who know what you could do with these?

Note that in building a “frabric” you could build a flexible system, not a rigid one, with a lot of microcomputer control.

NOTE: I now believe this idea won't work.

The basic problem is that I now know that propeller efficiency is 80% to 90%.  Although the “air claw” or “air treader” could in theory have a higher efficiency it seems like the chance of having much success this way is very unlikely.  Given that propellers are 80% efficient and airfoils have a lift-to-drag ratio of 4 to 10 to 40, over all flight in a rotary craft is probably very efficient.  The possibility of increasing efficiency very highly is very low.

I may now think about attempting to generate a 3-d array of many very small ducted fans, for example.

An additional idea that might be valuable for solar power, and has the advantage of safety, might be called the “big safe drogue pump”.  This would be the idea of having at least one drogue in a fixed position and bring another closer to it, creating a pump that pushes air downward.  Then one of the drogues would be open at all times.  This is not so different than using the thunniform motion idea.  After we prove that we can get that working, we could move the drogue shape to more of a foil shape.

Note also that we would like all of this to work in the “vector equilibirum” shape for safety, which provides a of travel in each direction.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #6: "Air Treader", resistance-based flight</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

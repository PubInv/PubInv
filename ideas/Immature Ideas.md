# This is a file for ideas which I have not yet researched.

## Idea: Could we build a smokestack flare igniter? 

The idea would be to put an "egg beater" style turbine (it would not
have to be efficient) in the pipe, use it to charge a capacitor, voltage regulate it enough to drive an Arduino,
use a transformer to fire a spark to ignite exhaust gases? This would be very valuable for my "biochar producing" oven.

## Idea: Sensor blinker

Could we build a "blinker", a cover that would briefly open to allow a sensor to take a reading or a spark to be 
applied in a very hostile environment, like the underside of a working lawnmower or the inside of a smoke stack?


## Idea: Make an accurate physical simulation of a biochar retort

Build a D3-based usable simulation of a biochar retort, using a true physical model that was fairly 
accurate in terms of heat produced and gas flows.  This would be both a design tool and a valuable educational 
tool.

## Idea: Improvements to the Biochar Retort

* Make a one-time O2 shutoff.  You "cock" a sliding door open.  An Arduino uses a solenoid to "fire" the cocked door
and gravity slams it shut.  As a safety feature, once you shut it, you never open it (until it cools down.)

* Make a single valve that controls the proportion of syngas going to the waste flare or to the retort.

* Use either the egg-beater or an actual heat engine to power the Arduino to measure and control temperature 
and shut off the O2 and possibly control the single exhaust valve.  This same power could spark the syngas in both 
the exhaust flare and to the retort.  The result would be a systme that has no battery power.  You literally just
light the fuel with one match and it does the rest.  

Obviously, all of this is taking place in a very hostile environment --- not sure how well that will work.  I guess
we may fint out.

## Idea: Detect bacteria by detecting a dielectric change

Our ability to analyze water quality is seriously hampered by the fact that we use indirect methods that are very slow.

I believe a bacterium is on micrometer in size.  We can make microchips with features much smaller, 14 nanometers.  What if we made a microship that was a two-dimensional grid that had a capacitance contact in each cell?  Then we 
cover the grid with water to be analyzed.  We then freeze dry it to remove the water, presumably leaving bacteria
in place. Then we measure the capacitance of each cell (possibly doing this at wide number of frequencies, since
permittivity is frequency dependent.) We expect most cells to contain pure water.  Some cells will presumably 
contain dirt. Some will presumably contain a bacterium, and possibly we can detect this by the dielectric constant (or graph.)

Reference: http://www.microwaves101.com/encyclopedias/measuring-dielectric-constant

## Idea: Stove-pipe microgenerator

It would be really nice to extract a small amount of power (about 1 Watt, enough to drive an Arduino, 100 milliamps at 12 V ~= 1.2 W) from a stovepipe/smokestack.

This could be done by placeing a turbine in the flow.  However, that would be a hostile enivronment.  What we would
really like a something that we can just clamp onto a warm pipe to produce enough power to trickle-charge a battery,
to supply intermittent power to a microcontroller.

Obviously, this could be done with a stirling engine of some kind.  But we are talking about pretty low temperature
differential here, and there is not much point if it costs more than $50.  However, the pracical uses for this
kind of micro-generation of power are quite great, and learn how to do the engineering reliably might be quite a
challenge.

An alternate idea is a micro-generator that can extract power from very weak air flows.  For example, could we put 
a computer-cooling fan size turbine in a pipe and let either composting gases or just the occasional gust of wind
provide power for it.

This gentlemen is doing something similar (bigger and requires fuel.) https://www.kickstarter.com/projects/672465444/low-cost-sterling-engine/posts/720042

Here is another reference:

http://www.scraptopower.co.uk/can-stirling/build-a-stirling-generator

## Idea: Lily-pad based force sensors in martial arts gloves

This idea was just inspired by the "Lily-pad" board for the Arduino, which is very small and supports "wearable" computing.  We could imagine a set of "boxing" gloves (I don't know what you call the gloves you use to protect your
hands when hitting a heavy bag) that measure the force/impact in each strike using a force sensor and somehow 
records this and let's you get feedback and review.

I'm not much of a martial artist, but I know a lot of people would like to know that they threw "30 heavy punches" in a three-minute round with a heavy bag.  I have no idea what a "heavy" punch is---but we could use force sensors
to quantify this.

## Idea: Unstable plane-in-wind power generator

Out where the tumbleweeds roll, they put signs on the ground to advertise gas stations. These are loaded on a spring, because the wind would blow them over otherwise.  It is windy on the plains, and they quite often are blown flat but they pop right back up.  Under some wind speeds they oscillate noticable.

We could put a magnet-and-coil system in the base of these to generate power.  It is hard to imagine this being as effective as a turbine, but small is beautiful. Perhaps such a system would be better in some location, where a turbine might harm a child or a bird, and where you can't build very high, or where the wind is highly unpredictable.

Possible such a system would work in flowing water as well, more reliably than turbine, that would be damaged by logs and snags and aligators.

## Idea: Multi-axis Rotational microgeneator

I've heard people use a tiny magnet on a little cantilever to generate some microwattage for sensors.  This generates power from vibration.

Building on the idea above, what if we place a spherical magnet inside a set of coils and tried to build a "rotational microgenerator".  I haven't researched this yet, I assume it has been done.  Not so different than self-winding watches, which we have had for a century, I imagine. (This is close: http://www.kinetron.eu/micro-generator-technology/)

Note that I don't mean rotation in one dimension---I mean complete sperical rotation.  So if you had it in your front pocket, the gentle swaying of your leg, maybe a 10 degree change per step, would provide power, no matter how it was oriented in your pocket.

Joke: We could put this inside a Doc Halliday cutter and generate power that way --- not that his cutters don't have enough power!

You could mount this on a sqirrel, and use it to power a miniature "squirrel cam".  The squirrels in my back yard spend a lot of time changing direction!  It would be pretty fun to see the world as a squirrel---they fly, but along bent branches, not in a straight line.  A roller-coaster ride.  Now if I can only build an air rifle that will fit the camera and generator onto them....

Note: You could do this with 3 ring rotators in 3 perpendicular planes.

Note: It is simpler to extract energy from a change in rotation than from constant rotation, which requires some sort of external friction force.

## Idea: Solid-state breadboard

I've been doing a lot of breadboarding on an Arduino. It is easy to make a mistake, and it wastes wires, and it is hard to see, and it is too small.

I wonder if we could build a solid state breadboard that would handle the connections for us?  Perhaps it could even identify compoonents for us, and automatically provide places for O-scope probes.

* * * 

After thinking about this some more, it is clearly possible to build a "wireless" breadboard.  If you want to have 10 "slots" in the breadboard, you would ONLY need ~100 relays.  This sounds a little crazy, but it might be possible. I imagine a system in which you use LEDs to show which rail is "wired" to which other rails.  Then instead of jamming unreliable little wires jumpers into the system, you could actually program the breadboard configuration with an Arduino.  Which means of course that you could program it with a full-on computer---perhaps integrate with Fritzing.  It could be a very educational system.

100 relays for 10 slots (In general, you need N * N - 1 relays to make all possible physical connections.)  At the risk of reduced flexibility you can reduce the asymptotic complexity.  For example, you almost certainly don't need a a full 20 slot system --- you could have two 10-slot board areas, with a few rails available for communication between the two areas.

I suspect this could also be done with a FPGA --- but if you do that, you may be limited to CMOS logic voltages.  You would have a hard time adding true power applications to that.  However, I could be wrong---certainly, if you used MOSFETS you could go up to 60V and 30A, although I don't know if there would be affects at low and reverse voltages---relays would avoid that problem completely.

Perhaps there is some switching theory that would let you decrease the asymptotic complexity as well---off the top of my head I don't know it.  You might be able to make the number of relays limited to K * N, where K is a constant and N is the number of components you are tryin to breadboard.

This would be a fun project, and the result would be salable, if only for education purposes.

## Idea: Build a MOSFET-And-Sensor breakout board.

At Sparkfun and Fritzing, there are is a lot of open-source sharing of designs, some of which are in a form that things can be easily ordered as PCBs.  Commonly shared valuable designs include "Breakout boards" which make it easier to mount sensors, for example.

I find myself right now in need of something fairly generic: A breakout board that has a MOSFET, a (potentially) high voltage input (by high I mean up to 30V, higher than an Arduino) and a place to solder a sensor.  In my case, thise is a sensor uses one +5V rail, and ground rail, and brings back a signal in the 0V to +5V range.  I think this is something than many other people would use.

## Idea: Micropower to pump hot water for neonatal heating

Possibly we can move a great deal of heat by using a very small pump attached to a large pot of water.  If this could be done at cell-phone level milliwatttage, we might be in business here.

## Idea: (Born of frustration) Can someobdy please build a solid-state breadboard?

## Idea: Oscillatory cryotherapy and heat machine (probably done)

I'm sure somebody has had this idea, but a "pad" that oscillated relatively rapidly (say 60 seconds) between ice cold and very warm could be a pleasant therapeutic device.  I suspect this alreayd exists. Certainly the principle is not new, it would just be the implementation that would matter.

## Idea: A low-battery Buzzer for the Arduino

Today I ran down a 9V battery leaving it plugged into my Arduino.  Although there are lots of things you can do to decrease power, they are a little cumbersome.  But in anycase you will always run out of battery power eventually.  The Arduino allows you to read its own power voltage. Most batteries have an approximately flat but slightly decreasing voltage as they age.  The Arduino UNO has an on-board voltage regulator.  Either reading the input voltage to the regulator (might require a circuit) or the regulated voltage would give you SOME warning that you could hook up to a buzzer.

My experience at Austin Mini Maker Faire has led me to believe even further that this is a very vaulable, very reusable project. I think this should be given a high prority.

## Idea: String-art percussion musical instrument.

String wires across a frame in such a way that a large a number of wires are exposed to be played by striking with s drum stick.  For example, build a frame about 1 meter square, and string 40 wires around it such that they form an 40-sided polygon.  A musician can take a drumstick and strick any of the 40 wires individually.

## Idea: Multi-gas sensor

There exists a number of relatively inexpensive gas sensors sold by Sparkfun, for example.  They have part numbers like MQ-2 through MQ-9 and MQ-135.  These sense concentrations for various gases.  I doubt this is as valuable as spectroscopy or gas chromatography, but it having a portable instrument that showed you the read-outs of a variety f these sensors could be quite valuable.  It is possibly that after building such a device we would discover uses for it which are not apparent on first thought.  Many of these sensors have somewhat overlapping sensitive to various volatile gases, but one can imagine that possibly a certain amount of data analysis could allow you to tease out the relationships between various gases.  Each of these sensors cost about $5 (and up to $35).

## Idea: Stirling Egine displacer phase done electronically...

Stirling engines (http://en.wikipedia.org/wiki/Stirling_engine) are heat engines valued for their simplicity and robustness.  They basically rely on a physical mechanism to keep the displacer 90 degrees out of phase with the power piston. This is done with a linkage in most examples.

However, I wonder if we could build a Stirling engine that had two free pistons, both of which tied to so-called linear alternators (that is, they generate EMF directly by pushing a magnet into a coil, and move the displacer 90 degress out of phase with the power piston?  That is, for example, could we use either a properly designed circuit to do this, or perhaps even a microcontroller.

Making a 90-degree phase change in a continuous AC current is in chapter one of Horowitz and Hill.  I'm afraid I'm not smart enough to immediately see if this can be done in a non-continuous way with a simple circuit.  Clearly it can be done with a microcontroller if we have excess power (for startup only, it should generate power once it is going.)

This would potentially allow you to build very small Stirling engines, possibly in multiples.  One can imagine "printing a sheet" of Stirling Engines, which could then be wrapped around an exhaust pipe to make micro-power.

Upon reading further I believe this all old-hat and has been exhausted by others.


## Idea: Can we pump ferrofluids around with coils?

If we could, then one can imagine a wide variety of applications that could almost be printed much as a Printed Circuit Board is printed.

## Idea: Reliable instant-on power generation with bimetallic valves

A basic problem is how to reliably "wake up" a heat engine when the heat source is hot enough to provide power. The Stirling engine, for example, often must be primed by initiating mostion.  We would prefer a system that could stay cold and dead reliably for months and then begin extracing power reliably when the heat source gets hot.

I think this is a rather difficult problem, but the best that I can come up with is to keep a gas chamber perfectly sealed until a sufficient temperature difference for power extraction is obtained.  The only way I can think to do this very reliably is with a bimetallic valve which keeps pressure very solidly until opening when hot.  Possibly such things already exist.

If we had a valve that waited until X degrees of temperature difference existed and then would stay open until (X-K) degrees of temperature difference existed, we would have a very reliable system.

## Idea: Phased Array Sonic Micro Communication

WiFi is an excellent communcation mechanism.  Wifi chips and shields are available for the Arduino.  I wonder if we could build an inexpensive system with mere microphones that could "find" each other in space, so that two Arduinos could communicate with each other?  This could be conceivably be done with small phased arrays of microphones.  I'm not sure this would really be better than radio communications---but at least it would be interesting. In theory this could be done very very inexpensively.

## Idea: Multi-pole Latching Linear Actuator

I've actually started working on this in Spring4.md.

## Idea: Linear Induction Motor for Linear Actuator

Last night my friend John Gibbons asked in an off-the-cuff way, "Why not use a linear induction motor?" for the Actuator. At the time I didn't understand what one was. I now believe this is a valuable idea. Unlike the Multi-pole latching linear actuator, it will require more than one electromagnet.  However, it would have the advantage of smoother operation, whereas my multi-pole latching linear actuator is, well, multi-polar.

## Idea: Make a photo mask with Ferrofluid by using currents in a thin capillary surface

If you enclose ferrofluid in a clear plastic bag, you can move the ferrofluid around with a magnet.  It actually 
requires a surprisingline strong field to do this.  However, possibly it would require less if we used glass.
If we put a drop of ferrofluid on a microscope slide, we might be able to design a pattern using a a grid of 
electrical wires and then, for example, lower the temperature to make it more stable.  This could then be used
to make some sort of photomask.  Possibly this would be far moreinteresting when done on a smaller scale.  
A variation of this idea would be to impregnae a cloth and attempt to concentrate the ferrofluid with the same approach, possibly producing a controlled pattern.  Possibly this could then be used to dye selectively.

![imag0179](https://cloud.githubusercontent.com/assets/5296671/7817261/7a6d9d88-0399-11e5-8b10-39842779a875.jpg)

## Idea: Make diffraction grating or a hologram with Ferrofluid

Is this possible? I would start by attempting to make a diffraction grating. (Note: After research, it looks like this has been attempted: http://webcache.googleusercontent.com/search?q=cache:pr0xXrnKJLkJ:piers.org/piersproceedings/download.php%3Ffile%3DcGllcnMyMDE0R3Vhbmd6aG91fDFQMF8wMDYwLnBkZnwxNDA0MTQwMzE0NDY%3D+&cd=1&hl=en&ct=clnk&gl=us&client=safari, as a google search reveals.  A cursory reading of this paper raises a number of questions.  I believe this is something that could be experimented with in a home laboratory very reasonably. Note that it also raises the possibility (that I had not considered) of simply building a magnetic controlled lens at a macroscropic level.

## Idea: Could we make a very small, light movable stage with ferrofluid?

Could we treat ferro fluid as an ink, print dots on a page, then use an electronic magnet to move the page in two dimensions?

## Idea: A fluid cooled coil system....

The way we build coils now is ridiculous---we use copper wire that is heavier than we really need, decreasing the number of turns we can put on a coil, because we can't keep the coil cool.  Someone needs to figure out a robust fluid based coil.  Could we 3-D print a spool that has nice little air or water channels build in?  Could we use bare copper wire inside some fluid guaranteed to be non-conductive?  It would seem that this would overall be a huge money saver.

## Idea: Build a Burrowing Robot

![burrowing robot](https://cloud.githubusercontent.com/assets/5296671/8398720/1dab4870-1dc0-11e5-9e39-5a07ba482572.png)

I think it would be pretty cool to build a burrowing robot.  There are many uses for this in terms of investigating buried archeaologoical sites, following pipes looking for leaks, mapping animal burrows and root systems, taking sub-surface soil samples.  And truffles---did I mention truffles?

I don't know if people have ever built such a think before.  Based on the diagram above I think it could basically be done with solenoids only, though of course refinement is possible.  Such a device could burrow through sand.

We might even imagine taking a tough bladder full of wax and filling it with burrowers, and using the burrowers to move the bladder/membrane---an artifical slime mold if you will.  BTW, sonic communication would be a good way to communicate with the robot while underground.

## Idea: Distillation in a Suitcase

I was at dinner with my friend John Gibbons and I came up with the idea of a "Chemical Synthesis plant the size of breadbox".  That's a nice idea, but its hard to imagine how to really make it, given the wide variety of feedstocks required.

A simple idea is to build a "Refinery in a Suitcase".  Even simpler is a "Still in a Suitcase".  You could pour in a heavy hydrocarbon and get out oil, and gasoline, and tar, etc.  You could pour in "beer" (by which I mean fermented vegetable matter to the limit of alcohol or vinegar production) and get out a concentrated product.  I don't mean a "still" for making whiskey per se, but something precisely controlled.

## Idea: Build a Machine that Gives you Anything you want that you can mount on telephone poles

Okay, I admit this is wacky---perhaps it is more of an art project than anything else.  The basic Idea would be a machine that says a sign that says "What do you need?" and some buttons:

* Food : You press this and a nutritious energy bar pops out
* Water: Your press this a cold drink pops up
* Information: You press this a book pops out
* Love: You press this and a small stuffed animal pops out
* Courage: Your press this and you get an inspiring quote
* 

## Idea: Make a slowly switchable magnet out of multiple rare earth magents that can rotate.

The fundamental beauty of the electromagnet is that it is controllable.  The fundamental beauty of the rare-earth magnet is that it is strong and permanent.

Iron consists of tiny domains which can be switched very rapidly to line up in the same polarity, adding up to a strong field.  This can occur very rapidly---at radio frequenicys of MHz, I think, certainly 100s of KHz in transformers.

Suppose you had a matchbox filled with tiny, 1/8" by 1/8" neodymium magnets.  Without moving the matchbox itself, you could change the polarity by turning each tiny magnet around 180 degrees.

Of course, it wouldn't stay put until more than half of the magnets are switched!

But, if we had an electromechanical means of controlling and locking each magnet, then we could potentially switch and lock each magnet individually.  We would then have a very strong magnet that we have switched (albeit rather slowly) to the opposite polarity.  But once we have done so, it requires not power.

## Idea: Use OpenSCAD to make parametric fractal trusses

There has been a lot of research into microscopic truseses, including those that exhibit a fractal nature.  OpenSCAD is a parametric system.  A Plug-in or something that you let you take any two points and join them with a fractal truss could be beautiful, wicked, and highly strong and highly efficient.  This would be a pretty easy project --- medium computer skills, and a lot of patience figuring out how fine you could print, and perhaps some analytic work to measure if it was really stronger in some way.

## Idea: Build an "auto octet-truss" system to turn planar surfaces into octet trusses.

## Idea: Even simpler: Just put a proper octest truss design at Thingiverse!!

## Idea: Build an easier to cool electromagnetic coil by using solid discs and a chopper circuit

This is based on the idea of a Bitter magnet.  One of the main limitations of electromagnetic coils, which are normally made with coiling wire or magnet wire, is that they get too hot. It is hard to get the heat away from them. This can be addressed by various heat sinks, or even putting tubes filled with water into the coils to provide water cooling.  But these are relatively complex solutions.

What if instead we manifactured a magent with justs discs of paper think copper?  We spaced these with little pads of insulation which kept them from shorting, but allowed a fluid (air, preferably) to be forced through them efficiently. Since copper is a good heat conductor, air against a multitude of thin plates would be a great heat conveyance mechanism---in fact, that is how heat sinks are built.

The result would have the problem that it would have almost zero resistance, which would mean that it would be almost a short circuit for your power source. It would draw a very high amperage, limited probably by the internal resistance of your power source.  To solve this, we would feed it with a capacitor.  That would of course also melt the capacitor---if we let it run for long. But if we had a chopping circuit that would pulse it, perhaps with a small duty cycle, we might be able to tolerate the high amperage, because we would be dividing it by the duty cycle. MOSFETs are capable of very rapid switching.  However, they themselves are current limited. But in principle, if our chopping circuit and our capacitor could survive the current draw, we might be okay.

The result would be an electomagnet that was effectively "pulse width modulated". It would have a single "winding", compared to a wire coil, so the number of turns would be small (perahps 2-10 per millimeter of length), but the amperage would be high. Taking heat out would be relatively easy. 

# Idea: (ART) Build a coffe table that has a glass-covered stream table.  A pump would inject water at one end, which would flow down hill.  This would naturally createa river-delta pattern of deposition and erosion.  It could be quite beautiful. Some variation in the flow would simulate flooding.  This could be accomplished pretty easily (say $2000) and would make a very educational gift.

# Idea: Volumetric colony counting.

I've been studying bacteriologic analysis of water quality as part of my volunteer effort for EWB.  Petriflims, produced by 3M, are one way of doing this.  They have the advantage of being quantititave, but they have some limitations.  In particular, each film can only measure 1 ml of water, which means that a moderately high contamination level is required.  I think we could just create a volume, like maybe cube root (10 ) centimeters to produce a 10-cc volume. We should in theory be able to move the focal plane of microscope throughout this volume, building a volumetric map of colonies within the volume.  Alternatively, we could incubate a volume and extrude it into a thin plane that we can count with a microscope very easily.

# Idea: Magnetically coupled reconfigurable self-sending robots...

Following my work on the "gluss" robot and Robert Gatliff's suggestion to use a "geomag" like system, build a a joint based on magnets that can couple to steel balls. Add to this an electrically signal of some kind that allows each actuator to determine which actuators it is connected to. Thus a person can easily assemble and dissassemble it by hand, and it automatically recognizes the geometry.

# Idea: Build a better Tea Infuser

I got my wife a nice tea infuser for Christmas.  However, a better one would tell you the temperature, have preset steeping times based on the kind of tea, and control tea and temperature.  This is actually a pretty easy and slightly awesome project. 

# Idea: Write software to automatically carve 3D printable object into smaller pieces

This would allow large objects to be created conveniently.  It would involve some "joinery".  Probably has already been done.

# Idea: Create simplist possible heat pump

As part of my work for Engineers Without Borders, I am making a petrifilm incubator.  This uses Joule heating to keep things at approximately body temperature.  However, it has no way of cooling.  It might be both more efficient, and possibly capable of cooling, if we had a miniature, battery powered reversible heat pump.

# Idea: Create an OpenSCAD parametric Truss

The idea would be to make a customizable truss, using the principles of the Octet Truss, to allow a truss of any dimensions to be 3D printed. Thus if anyone wanted a strong part that fit within their printing capabilities, they could easily build it to the exact dimensions that they need.  This is great idea because it is so simple -- not really an invention at all -- more of an open-source contribution to the world of 3D printing.

# Idea: 3D Print Vascular Net as a Heat Exchanger

3D Print vessels containing one-way pasive leaf valves, much like the human blood vessel.  See if we can then use simple heat to drive the motion of a fluid. This is slightly crazy, but Nylon melts at above 220C, and water boils at 100C, so the possibility exists that we could build a nylon system of vessels containg water that would circulate completely passively due to expansion and release of steam in indvidually cells opened by valves onto the next cells. This could then be used as a passive (and very cheap) heat exchanger. It could even do somethign crazier, like maybe make a cooking vessel that could withstand flame.  That sounds crazy, but we have all seen the experiments of boiling water in a paper cup and know that ancients used to use an animal skin as a cooking pot. So long as it stays moist to prevent the temperature going above 100C, this could work.  Imagine if we could 3D Print a Tea Kettle that we could actually place over a gas burner!

# Idea: Develop an Abstract Data Type that does a good job representing Conservation Laws

Conservation laws are useful in many situations: double-entry bookkeeping, games, angular momentum, linear momentum, mass, energy, etc.  Yet we do not have a fundamental, cross-language Abstract Data Type to represent a Conserved Quantity.  This is a great project because it could be applied to many different langagues.

# Idea: Investigate the periodicity of convergenet series

I know this is probably well-knwon, but looking at the series expansion of the SIN function it is just very unnartural to see that it has a period of 2PI. For example, we know SIN(1000) is something in the range [-1,1] but the first term is big. I don't have the knowledge to think about this but as a computer scientist it seems wrong.

I know I really need to take a full course in analysis.  There is so much that I don't understand.  But I am still mystified by the series expansion of sin x, and how it can be period, and how it can generate such huge numbers which all cancel out. It seems to me there should be some way of representing it that captures its essential nature better than the awful power series. Also, I am intrigued that the truncated power series expansion is completely rational if x is rational, even though in general we think of sin as producing a rational result only if the input is a fraction of 2PI, and therefore transcendental. (This of course is a TRUNCATION, which makes all the difference, but still!)  This is probably just a mental weakness on my part somehow.  However, the fact that the expansion produces a "moving lump" like a wave packet is very real and I think requires some explanation.

# Idea: Put multiple objects in orbit such that they can "sling-shot" an object

In science fiction movies, one sometimes heres of the "slingshot" effect, which adds velocity to an object. In fact this nothing mysterious---a rocket temporarily allows itself to be captured by a fast moving object, like Jupiter.

Since Jupiter is so big, you can gain energy falling towards it. Since it is orbiting the sun, it has a high velocity relative to the sun. While captured, a rocket has this velocity. If the rocket has chosen an orbit correctly, it can then escape 
from Jupiter's gravity having some of Jupiter's velocity, even though the act of escaping slows it down.

Suppose we had a tremendous (dare I say God-like?) power to build a solar system. We start with a star. We add a Jupiter.
In orbit around Jupiter we place an object much smaller than jupiter orbiting in the same plane, at a great distance. Then around that object we place another object orbiting at great distance.

Could we then have a rocket maneuver so that it successively sling-shotted by these smaller and smaller planetoids, thereby effectively gaining the absolute velocity of the last planetoid at relatively little energy expenditure?

# Idea: Ferrofluid amoeba

If you had a bag half-filled with ferrofluid, with coils attached all over the surface, a careful control of the energized coils would allow some eversion or motion of the bag. Possibly you could build a moving "amoeba" in this way.
The coils could detect each other by sensing induced voltage; this would possibly allow a spatial model of the bag to be internally constructed.

A simpler version of this would be to make tube and see if you could get it to roll.

Note: I tested this idea and it basically won't work with just ferrofluid, or not easily---the ferrofluid by itself does not have enough iron in it to make powerful enough magnets for this to work.

# Idea: Ferrofluid tentacle based on a "spine"

We could 3D print an object holding 3 bobbins for magnet wire coils. The center could have one male and one female part to construct a "spine" or pieces fitted together. An elastic "ligament" would hold these together. If this spine were immersed in a flexible tube of ferrofluid, then the spine would 
have flexing pressure when the coils have current. This could be either repulisve to drive the coils apart (on one side) and/or attractive (on the other sides.) The 3 pairs of wires could be routed through the central holes to form a "spinal column" allowing power to come from a single source. With a power multiplexer, this could be a relatively simple PCB; or a large number of transistors could be used.

# Idea: A Bag of Iron BBs as a ferro-"fluid"

It would be wonderful if we had a fluid that could form a magnetic core as good as soft iron---that is, which allowed powerful magnets to be constructed
with fluid-filled coils of wire. Ferrofluid by itself is NOT very good at this. Perhaps however, we could make a semi-fluid by making bunch of larger
iron particles (BB-sized shot) and suspeneding them in an oil. In all probability this would be a terrible "fluid" -- it would clump, and be affected
by gravity. However, under specific conditions (such as the whole container being filled), it might be a reasonable "soft" and movable system.

# Idea: Parallel Magnetic Plates for Making a Ferrofluid Piston

In order to use ferrofluid, you often want to create a "piston" that can be used to push air or an immiscible fluid.
The obvious way to do this is to use a cylinder with a bolus of ferrofluid driven by horseshoe magnets arrayed along the cylinder.
However, a potentially more powerful is to create a magnetic circuit by using actual iron plates or bars (that is, in contact with
the fluid, so perhaps INSIDE a cylinder. The idea is that by simply magnetizing these plates, you create a magnetic circuit
that creates considerable force to be filled by ferrfluid (that is, the fluid wants to fill the gap.)
The question is: Can you make a more powerful "piston" this way?  An additional question is could these plates be shaped,
such as triangles, in order to allow a changing force profile.



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH: Immature Ideas</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

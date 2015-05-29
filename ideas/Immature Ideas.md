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


<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH: Immature Ideas</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

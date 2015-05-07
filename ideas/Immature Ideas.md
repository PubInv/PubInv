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

## Idea: Build a MOSFET-And-Sensor breakout board.

At Sparkfun and Fritzing, there are is a lot of open-source sharing of designs, some of which are in a form that things can be easily ordered as PCBs.  Commonly shared valuable designs include "Breakout boards" which make it easier to mount sensors, for example.

I find myself right now in need of something fairly generic: A breakout board that has a MOSFET, a (potentially) high voltage input (by high I mean up to 30V, higher than an Arduino) and a place to solder a sensor.  In my case, thise is a sensor uses one +5V rail, and ground rail, and brings back a signal in the 0V to +5V range.  I think this is something than many other people would use.

## Idea: Micropower to pump hot water for neonatal heating

Possibly we can move a great deal of heat by using a very small pump attached to a large pot of water.  If this could be done at cell-phone level milliwatttage, we might be in business here.

## Idea: (Born of frustration) Can someobdy please build a solid-state breadboard?

## Idea: Oscillatory cryotherapy and heat machine (probably done)

I'm sure somebody has had this idea, but a "pad" that oscillated relatively rapidly (say 60 seconds) between ice cold and very warm could be a pleasant therapeutic device.  I suspect this alreayd exists. Certainly the principle is not new, it would just be the implementation that would matter.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH: Immature Ideas</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

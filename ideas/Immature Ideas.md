# This is a file for ideas which I have not yet researched.

## Idea: Could we build a smokestack flare igniter? 

The idea would be to put an "egg beater" style turbine (it would not
have to be efficient) in the pipe, use it to charge a capacitor, voltage regulate it enough to drive an Arduino,
use a transformer to fire a spark to ignite exhaust gases? This would be very valuable for my "biochar producing" oven.

## Idea: Sensor blinker

Could we build a "blinker", a cover that would briefly open to allow a sensor to take a reading or a spark to be 
applied in a very hostile environment, like the underside of a working lawnmower or the inside of a smoke stack?

## Idea: Arduino control game

[123D Circuits](http://123d.circuits.io) has some WONDERFUL Arduino simulators.  Could we build a "game" out of
one of their simulators?  The idea is that we program and Arduino to intentioal represent an unstable behavior control
problem.  We would have a hidden internal model.  We produce a single output voltage that is "where we are".  The 
player must build a second Arduino which supplies a single input voltage to the unstable control system.  The goal 
of the game is to keept the unstable system close to some central value.  However, we don't tell you how 
we are going to react to your input!

But we do give you some parameters.  We will change our model smoothly and no faster than a certain rate per second.
So if a "high" input is driving us "high" this turn, way may change that next turn, but only at a gentle rate. After 
five or 10 seconds, a value that was driving "high" at a fast rate will now be drivin us "low" at a fast rate.

This could LITERALLY be done as simulation at the above site, and people could fork it and try to program the 
second Arduino!

This would apply to all kinds of control problems, such as keeping a neo-natal incubator at a correct temperature, 
or controlling a fire within a temperature range to produce good biochar.

## Idea: Arduino sketch sketcher for Homeostasis

Build a D3-based software system that lets you automatically generate plans that make solving a "homeostasis" problem with an Arduino easier.

Many problems that you wish to address with an Arduino can be valuably charactized as a variant of the problem of maintaining some conditions (homeostatis).  For example, the premature infant incubator problem is one of maintaining the incubator at 37C within fairly narrow limits. Although not particularly difficult if you are a skilled programmer, we can imagine a website (publishable here on GitHub) that makes it even easier.

We could have a D3-based visual system that allow you to drag-and-drop from an expandable palette of sensors, remediators, and strategies.  Although we can allow new sensors to be added, we can prepopulate with some basic sensors such as the MQ4 methane sesnor and a basic temperature sensor.  Remediations could include "running a fan" or "sounding an alarm" or "turning on the heating coil". A user may choose a remediation strategy such as "turn on remediation #1 for 10 seconds and 80% power"

After the user sketches the system visually, the output includes:
* A bill of materials,
* An explicit sktech that can be downloaded directly into the Arduino, 
* A library-based Arduino sketch,
* A schematic, and even
* A printed circuit board---this would be pushing it!

### RemeDI: A Digital Interface like MIDI for Arduino sensors

A part of this idea would be to provide a "Digital Interface" to each kind of sensor.  This would be an expanding library, but it would allow each sensor and remediation to be treated in a fairly standard way.

An important aspect of this would be to create an "event driven" approach.  (Probably a library for this already exists, I need to research.) We could treat each sensor as if it produced Events, and allow you to register Event Handlers for each of these events.  A typical Event would be "Temperature got too hot" from the TN335 sensor or "the push button was pushed". Programming could then be thought of in terms of creating event handlers.  The Remediation Actions (Or perhaps just "Actions" is a better term) would Also have a digitial interface, so you would call "Turn motor on for 3 seconds".  The library would have to handle the interlacing of time so that multiple actions could be handled at various times.

Note: It appears that QP, and possibly other solutions, already do this. http://www.state-machine.com/qm/  At least they doe the Event-driven stuff, ad preemptive multi-tasking.  It is unclear how much they are handling the other idea of standardizing the physical sensors, but possibly quite a lot.  It is unclear that they focus on homeostasis or use the physical model of variables/remediation that I was thinking of, but clearly I will need to investigate.

Upon looking over QP, I infer:
* It is focused on State Machines, a valuable usecase but not quite the homeostatis issue I was looking for,
* It pushes you into the C++ domain, which seems unnecesary,
* You have to download the software,
* It is representing the resulting programs as XML, which presumably puts you most in the QP domain, and
* I didn't see anything that really addressed the sensor encapsulation problem.

So although I need to do some more research, it seems like a D3-based, generate the code for me, with a an emphasis on specific sensors, might be a very valuable addition to the space of Arduino programming.  I need to investigate this further.

Note that this library: https://github.com/igormiktor/arduino-EventManager seems somewhat simpler, but very similar in some ways.

Note: A firm, http://www.vernier.com/engineering/arduino/, Vernier, appears to have standardized their own line of sensors for the Arduino.  In that sense they may have done a lot of what we want here.  It is unclear how extensible it is.  People have built a "Vernier Shield", because most of the Vernier sensors appear to use their own physical public standard.

Note: A Dallas firm has created the "1-Wire" approach to building sensors --- basically they implement a simple digital protocol for the communication between the sensor and the system (possibly an Arduino.)  http://playground.arduino.cc/Learning/OneWire  This seems like a very nice idea but requires extra electronics on the sensor side.  This is not quite the "pick your sensor and software wrapper to make it look digital" that this idea was going for.

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



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH: Immature Ideas</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

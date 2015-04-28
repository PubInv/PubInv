# Homeoduino (Homeostatis with an Arduino)

There are many controls problems that can be conveniently thought of as "sense and react to this physical variable in order to maintain maintain homeostasis".

I believe this can be made easier if we produce some software tools for doing just that, and perhaps some hardware conventions.

Furthermore, I am currently working with Engineers Without Borders (Greater Austin Chapter) on three problems that are homeostatis problems, and a fourth for PIFAH:
* We are attempting to keep a latrine fresh by running a fan when we sense gases,
* We are attempting to build an incubator for premature infants that must maintain body temperature, and
* In order to test that we would like a "dummy baby" that proves its temperature has been maintained and for training, and
* Finally, my interest in pyrolysis can also be thought of a as a multi-phase stasis project (maintain temperature at 350 C until all syngas production is complete).

I think all of these ideas converge enough to warrant a complete repo for this.

## Idea: Arduino control game

123D Circuits has some WONDERFUL Arduino simulators. Could we build a "game" out of one of their simulators? The idea is that we program and Arduino to intentioal represent an unstable behavior control problem. We would have a hidden internal model. We produce a single output voltage that is "where we are". The player must build a second Arduino which supplies a single input voltage to the unstable control system. The goal of the game is to keept the unstable system close to some central value. However, we don't tell you how we are going to react to your input!

But we do give you some parameters. We will change our model smoothly and no faster than a certain rate per second. So if a "high" input is driving us "high" this turn, way may change that next turn, but only at a gentle rate. After five or 10 seconds, a value that was driving "high" at a fast rate will now be drivin us "low" at a fast rate.

This could LITERALLY be done as simulation at the above site, and people could fork it and try to program the second Arduino!

This would apply to all kinds of control problems, such as keeping a neo-natal incubator at a correct temperature, or controlling a fire within a temperature range to produce good biochar.

Note: The PID algortihm could be a potential candidate algoirthm for this, and there exists and Arduino library for it already: http://en.wikipedia.org/wiki/PID_controller

## Idea: Arduino sketch sketcher for Homeostasis

Build a D3-based software system that lets you automatically generate plans that make solving a "homeostasis" problem with an Arduino easier.

Many problems that you wish to address with an Arduino can be valuably charactized as a variant of the problem of maintaining some conditions (homeostatis). For example, the premature infant incubator problem is one of maintaining the incubator at 37C within fairly narrow limits. Although not particularly difficult if you are a skilled programmer, we can imagine a website (publishable here on GitHub) that makes it even easier.

We could have a D3-based visual system that allow you to drag-and-drop from an expandable palette of sensors, remediators, and strategies. Although we can allow new sensors to be added, we can prepopulate with some basic sensors such as the MQ4 methane sesnor and a basic temperature sensor. Remediations could include "running a fan" or "sounding an alarm" or "turning on the heating coil". A user may choose a remediation strategy such as "turn on remediation #1 for 10 seconds and 80% power"

After the user sketches the system visually, the output includes:

A bill of materials,
An explicit sktech that can be downloaded directly into the Arduino, 
A library-based Arduino sketch,
A schematic, and even
A printed circuit board---this would be pushing it!
RemeDI: A Digital Interface like MIDI for Arduino sensors

A part of this idea would be to provide a "Digital Interface" to each kind of sensor. This would be an expanding library, but it would allow each sensor and remediation to be treated in a fairly standard way.

An important aspect of this would be to create an "event driven" approach. (Probably a library for this already exists, I need to research.) We could treat each sensor as if it produced Events, and allow you to register Event Handlers for each of these events. A typical Event would be "Temperature got too hot" from the TN335 sensor or "the push button was pushed". Programming could then be thought of in terms of creating event handlers. The Remediation Actions (Or perhaps just "Actions" is a better term) would Also have a digitial interface, so you would call "Turn motor on for 3 seconds". The library would have to handle the interlacing of time so that multiple actions could be handled at various times.

Note: It appears that QP, and possibly other solutions, already do this. http://www.state-machine.com/qm/ At least they doe the Event-driven stuff, ad preemptive multi-tasking. It is unclear how much they are handling the other idea of standardizing the physical sensors, but possibly quite a lot. It is unclear that they focus on homeostasis or use the physical model of variables/remediation that I was thinking of, but clearly I will need to investigate.

Upon looking over QP, I infer:

It is focused on State Machines, a valuable usecase but not quite the homeostatis issue I was looking for,
It pushes you into the C++ domain, which seems unnecesary,
You have to download the software,
It is representing the resulting programs as XML, which presumably puts you most in the QP domain, and
I didn't see anything that really addressed the sensor encapsulation problem.
So although I need to do some more research, it seems like a D3-based, generate the code for me, with a an emphasis on specific sensors, might be a very valuable addition to the space of Arduino programming. I need to investigate this further.

Note that this library: https://github.com/igormiktor/arduino-EventManager seems somewhat simpler, but very similar in some ways.

Note: A firm, http://www.vernier.com/engineering/arduino/, Vernier, appears to have standardized their own line of sensors for the Arduino. In that sense they may have done a lot of what we want here. It is unclear how extensible it is. People have built a "Vernier Shield", because most of the Vernier sensors appear to use their own physical public standard.

Note: A Dallas firm has created the "1-Wire" approach to building sensors --- basically they implement a simple digital protocol for the communication between the sensor and the system (possibly an Arduino.) http://playground.arduino.cc/Learning/OneWire This seems like a very nice idea but requires extra electronics on the sensor side. This is not quite the "pick your sensor and software wrapper to make it look digital" that this idea was going for.

# References

Note: The "PID" project seems to be related:

http://playground.arduino.cc/Code/PIDLibrary
https://github.com/br3ttb/Arduino-PID-Library/


<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #26: Homeduino (Homeostasis using Arduino)</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>. 

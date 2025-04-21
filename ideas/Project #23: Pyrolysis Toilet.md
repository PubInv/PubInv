# An Approach to the "Re-inventing the Toilet" challenge of the Gates Foundation

## Basic Idea: Build a toilet that quickly pyrolyzes human feces to produce biochar

By completely pyrolyzing human feces we can render it completely safe and useful. This is an approach that could
be quickly adopted by the public due it its extreme convenience. In particular, we are attempting to design a system
that produces no sewage, which is valuable for freeing people from development grids. Finally, the treatment of wastewater
even in advanced nations creates terrible aquatic pollution and is expensive.

## Motivation

Sanitation is a huge issue. However, as suggested in another project, a toilet should also provide valuable health
information for its users. In partiuclar this project is a very Western-targeted, high-tech approach. This is counter-intuitive,
as it is not the developed world that needs better sanitation.

However, there are three reasons that this is a good livingry project:
* Computer control is in itself not expensive. Microchips are made from sand.
* There is a some social admiration for high-tech approaches.
* The project is water-conserving and carbon-sequestering.

## Motivation for Pyrolysis

Project #9 suggests the use of thermal depolymerization to eliminate human waste.

I now believe that for a single-person point source toilet would be better served by performing pyrolysis to produce
biochar.

The biochar is a more easily used end-product, and it doesn't not require high-pressure to produce.

Note that this project is strongly related to "Single chamber" pyrolysis project, as the prevention of a positive feedback loop 
as described there is absolutely essential. It is also closely related to the "Personal stool analysis" project.

## Implementation

The basic idea is to build a toilet that:
* Analyzes the stool producing valuable health information,
* Pyrolyzes it to biochar convenient removed from the toilet,
* Diverts urine to produce water and other valuable products.

So basically, I want to build a magic toilet that instantly hands you back a useful report, perfectly pure water, and a little baggy of powder
containing completely non-toxic powder that can be added to any garden.

And it is possible.

If we assume a high-tech solution to begin, with have a number of techniques open to us:
* We can use computer and sensor technology to do whatever analysis we want.
* We have electrical power to, for example, initiate pyrolysis.
* We can perform distillation.
* We can move the stool-containing container.

So, as a first pass, my basic idea is:
* Contain the feces and divert the urine.
* Analyzes both.
* Distill the urine.
* Use vacuum drying and RF heating to dry the feces. [This idea is now obsolete; I think this is wrong.]
* Pyrolyze it completely.
* Use motors to move the final product into a convenient packaging mechanism.
* Provide water for drinking or hand washing.
* Tells you precisely whatever you need to do for maintenance.

# Alternative Embodiment: Doggy Poop Scoop

Can we build a Doggy Pooper Scooper that is battery powered and uses RC heating to safely char scat?

The user experience should be: scoop, and by the time you get home it is completely dry and odor free.

# RF Pyrolysis

I have performed and planned some experiments with RF Heating (also known as dielectric heating.) In pursuant of that, I built a high-voltage power supply: https://github.com/PIFAH/PIFAH/blob/master/experiments/MIT-OCW%20High%20Voltage%20Power%20Supply.md
It is probably not quite up to snuff, as we really need a AC source at 10 MHz and probably more than a few Watts of power, but it is a start.

The reason I think this is interesting is that it may be a more efficient and safer way of drying feces and pyrolyzing it.  Since in any pyrolysis thorough drying is a necessary part of the process and major cost of the total energy, I would like to know if we can dry things using RF Heating (possibly in combination with a vacuum to lower the boiling point of water) efficiently and safely.  This may be safer than joule heating (or burning a fuel) because it is cleaner, can heat "from the inside" of the sample, and might prevent a dry crust on the outside from forming. Furthermore, although it requires high voltage, it might be safer overall than higher temperatures, in much the same way that a microwave oven (a related but distinct heating mechanism) is in someways safer than a gas overn.

# Thought as of April 21st, 2025

I currently believe we can try a simpler approach of using joule heating to repetitively raise the pressure with RF or joule heating, and then "flash" the steam off into a
safetly chamber at atmospheric pressure. I imagine that this will raise the pressure to 1-3 atmospheres above ambient pressure, and then opening a simple solenoid valve.
This approach will have to be done repeatedly until the sample is mostly dry. This makes for a simple mechanism and may work. I am now working with a volunteer to
do a mathematical model of this approach.



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #23:  Pyrolysis Toilet</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>. 


# Very Simple Heat Engine using bi-stable magnetic device

## Motivation

As mentioned elsewhere, I'm interested in powering an Arduino by extracting heat from a smokestack or chimney.
In general the field known as "microgeneration" is in interesting.

I was trying to create the very, very simplest heat engine that I could to provide about 1 Watt of power (about what
an Arduino draws, I think.) There are of course lots of heat engine, some of which are made on a tiny scale.
There seems to be an entire nice sub-industry building little steam engines and Stirling engines mostly for educational
purposes.  However, Stirling engines have a big flywheel, and seem to require something to start them off. I wanted
an engine that could lay dormant when no heat was in the pipe and then start itself up.  I'm afraid that is dependent
on having good air seals, but I have come up with an idea for a free-pistion egine based on the use of permanent 
magnets to create "bistable mechanical device". The permanent magnets are arranged so as to allow a build up of pressure,
and then to ensure that when the trigger energy is reached, there is enough power to switch the next part of the cycle.
This particular design uses two heat chambers, one of which is closed and one of which is open at all times, and the 
bistable piston guarantees that we are always in sone state or the other and never "stuck".

## Design

![rob design 001](https://cloud.githubusercontent.com/assets/5296671/7221423/192917a6-e6b0-11e4-9ead-130f6fab1018.png)

I don't know how clear this is from the drawing, but basically this is free-piston design.  We extract electric current when the magnetic piston moves inside the coil.  I don't actually understand the electronics of how to 
build the circuit for that, but I know it can be done.

We permanent magnetics to create bistable mechanical situation.  The piston cannot get stuck in the middle because
that is an unstable position.  The piston lenght is such that it always closes at least one of the ports to one of heat chambers, and since it can't get stuck in the middle, it will never close both for very long.

When enough pressure builds on one side, the piston overcomes the magnetic repulsion and "squirts" over to the other side. After it passes the magnet, the magents actualy help push it along with greater force.  As it changes sides,
it releases one chambe to the air (which could be a closed large volume or even open air), thus cooling it.  The other chamber is closed.  As the closed chamber is heated, it builds pressure, until the piston "squirts" back to the
other side.

In order to keep the piston from wacking into the walls and jamming, we can use additional permanent magnets to keep it from slamming into the end of the cylinder.

Although not shown, this could be a closed-air engine if we have a large enough "cool" chamber, but that is not technically needed, though it would increase realiability.

Perhaps it is not obvious from the diagram, but "N" and "S" in all cases represent the North and South poles of permanent magnets.  (Note that permanent magnets must be protected from heat.) I'm specifically imagining a relatively low heat differential for this system (to bleed power from a smoke stack or exhuast pipe, for instance.)

I'm excited about this idea and may work on it as the first sprint, though I have to order the magnets first!  




<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #24: Very simple heat engine with bistable magnetic device</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>. 

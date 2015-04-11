# Buckminster Fuller's Octet Truss

Buckminster Fuller invented the "Octet" Truss, which fills a plane with alternating tetrahedra and octohedra.
It is quite beautiful, and very strong.

# Robotics

If each member of the truss were not a rigid piece of angle iron but rather an extendable or contractible element,
then we can imagine the truss moving.  We could consturct a robotic truss.  Rather than a wheeled or walking robot, 
this would be a "flowing" robot.  It would move like a slug or a snake, which I why I call it a "Gluss" (slug truss).

# Construction

There are several well-understood and inexpensive models for the individual length-changing elements.  Hydraulic
cylinders are perhaps the most obvious. Solenoids have a completely different performance profile, because they are
fast but may require power to stay in postion. More generally this kind of device is called an "Actuator" and there
are many actuators for sale with many different performance profiles, strengths, sizes, and speeds.

# Computation

A Gluss cannot move by moving a single member, in general, as the Octet truss is a highly redundant and over-constrained 
mechanical linkage.  Rather, one would have to coordinate motion of several members at once.  The control of a Gluss 
is therefore an interesting problem. If we add in a realisitc situation that a few out of dozens of actuators are either
broken or behaving poorly, the problem becomes even more interesting.

The simple act of trying to figure out what posture the Gluss is in also an interesting control problem, that will
require a good bit of sensor/microcontroller skill.

Finally, the most valuable computational problem is figuring out a coordinated set of sequence to make it move 
in a valuable way.

# Motivation

A large Gluss made out of a few dozen hydraulic cylinders could server the purpose of a being an instant bridge.
When a bride a cross an uneven span is required, it could crawl across the span and position itself into a load-bearing
truss upon which a road surface could be placed.

A large Gluss could prop up a damaged and unsafe building.

A small Gluss could climb trees or climb into caves and other narrow spaces in ways that perhaps other robots could not.

Finally, this would just be a really fun project.

# History

Back in the early 90s with my friend Martin Smith, I hacked a program calles "XSpringies" to make a two-dimensional software gluss.  In this the actuators were not rigid but "springs", which made it easier.  I was able to make a little caterpillar-like gluss crawl across a virtual space through a serious of spring-length changes.  I did nothing more with the idea at the time.

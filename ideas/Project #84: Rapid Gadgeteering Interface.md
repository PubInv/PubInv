
# Rapid Gadgeteering Interface

A large number of devices which we might call "gadgets" are made by putting an microcontroller inside a controller with some sort of sensor
or control system. If we apply the "Unix Way" to this and attempt to make the most *physically* compositional system, much in the way
that software and electronic components are modular, we may obtain a modular system that allows extraordinarily rapid 
prototyping.

<img width="960" height="720" alt="RGI Drawing" src="https://github.com/user-attachments/assets/399e3908-7987-4c8a-97b2-c76a8c760908" />

I imagine small rectangle that can be physically composed by plugging some wires together and then sliding the parts together with 
a "dovetail" joint and the locked into place with long, slender bolts.

We can image a large number of physical gadgets that could be made if we had components for:
1. Battery power
2. An OLED or LCD screen  with a rotary encoder for menu selections
3. A speaker enclosure

Such a 3-component system, which would have a dovetail to accept new components, could create fully functional gadgets by 
adding new components, which would be releaved of some power management and GUI functionality. We could imagine:
1. a pulse-oximeter
1. A thermometer
1. A small digital 10X imaging system
1. A digital microscope
1. An unltrasound system
1. An retinoscope
1. A urinalysis system
1. A glycometer
1. A PCR incubator

... and, in fact, a gadget could be made which compbined ALL of these features!  Just as a "swiss-army knife" can have many 
blades, tools, and components, we could compose components in this way easily, though at the risk of the device becoming cumbersome.
It is almost always valuabe to be able to rapidly test a component, even if the resulting system, if manufactured, deserves a 
more specific and compact enclosure.

The electronic connects would also be standardized, including the physical connectors. For example, 12V, 5V, and 3.3V power lines
are very useful. SPI, I2C and USB can be used for communication between the components.

# Example

One of the enclosures that we have put a lot of work into is the Krake. There is no reason to throw away
this work, but we could redesign it as a componentized system. For example, we are thinking about 
adding a battery. If it were done as an RGI system, we could test the battery component without 
having to redesign the case---even if we planned to do make a perfect, compact enclosure later.

<img width="960" height="720" alt="Krake Redesigned at the RGI" src="https://github.com/user-attachments/assets/ce98771b-c076-43a2-be95-f87092a06dd8" />


# The Plan

This is just a sketch of an idea at present.  We can an artist to make a drawing of how this might work phycially, and what it would look like. 
We need electrical engineers and mechanical engineers to make precise how the interface would work.


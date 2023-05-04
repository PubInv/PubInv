# Greenwood Vessel Stove

About a billion people still cook everyday on a hand-gathered deadfall firewood. This is a time consuming drudgery and inefficient. Such wood has a low heating value,
and generally is not dried before burning, significantly decreasing its efficiency. 

Public Invention has another project, the EcoPot, which is an attempt to address this.

However, I am coming to believe that we need a stove-based solution.

![Greenwood Vessel Stove](https://user-images.githubusercontent.com/5296671/108615867-ead13080-73cd-11eb-8f05-7f80aa301f08.png)

Clearly, simply buying a people a $300 wood stove would, in fact, be a very useful starting point. In fact this would be an excellent use of $300B.
However, we may ask if we can design something that is efficient enough to be self financing, or better.

I believe that if we take the step of using a sealed reaction vessel for the combustion, then many improvements become possible.
We can use the reaction vessel as a vacuum dryer. We can further more treat the exhaust gases to abate smoke and other polution. Finally,
we can use forced air, or even O2 enriched air, to hasten and improve combustion.

The idea of using a PSA oxygen concentrator seems like economic madness; but I am not sure it is. My calcuclations suggest that under ideal conditions
only 26 grams of carbon are required to heat a 12-cup pot of water to boiling. However, this is not possible if you are heating an enourmous amount
of N2 in the air as a wasted flue gas.

So the basic idea is to make a sealed and carefully controlled vessel. To this vessel we attach a vacuum pump for drying, and valved exit 
flue for waste treatment, an air input port, and an O2 input port.

We device a solar-powered system that is in a sense optional: if we get no power, the system behaves as a normal stove. If, however, during the day
the sun shines and gives us 24V power, we use it to hold a drying vacuum on fuel, and possibly warm it. Possibly we can increase the pressure and
explosively release it to "puff" the wood, making it more porous, driable, and combustible. Drying takes time, but if cooking is a daily process,
we have time. Fuel is placed in the chamber in an untreated state and begins drying as power allows. Eventually, it may even be charged. If power allows 
and we have a O2 concentrator, we can store up compressed O2. At the time of cooking, the fuel is ignited and O2 injected up to the pressure and 
heat limits that we can tolerate. This requires careful control, but we have already commited to an electronic control system with sensors.

Using Pure O2 means the fire burns hot and fast; much of the heat will be radiant. But this will be captured in the stove and heat the stop top
without the loss of hot flue gases.

Eventually, we will be unable to add additional O2, so we open the exhuast port and take flue gases (which are now cooler due to time than they
would be if uncontrolled) into a pollution abatement exhaust system. This makes room for the injection of more O2 until the cooking is finished.
If we run out of O2, we can force air into the stove, which is less efficient but accomplished the same effect.

All of thise may seem like a ridiculous amount of sophistication for burning rotten wood; but I see it as a simple evolution of wood-burning technology.
This system allow nearly the worst fuel to be used by people who have no ability to obtain better fuel. It produces the lowest possible carbon footprint.
An initial cost estimate would be USD$5000 for such a system. However, like most things electronic, that cost could be radically reduced by engineering; 
a mass production price might be USD$500. 

## Initial  Experiments

I think this project could be begun by simpling investigating the power demands of vaccum drying on a small scale of deadfall wood.

For less than $200, you can buy a vacuum chanber used to degassing silicon molds. A fundamenal question is: Given a mass of deadfall wood, what is the drying time in such a vacuum chamber as a function of temperature?  In particular, acheiving a 4-hour or 8-hour drying time at a low temperature could be very useful. We can
control the temperature by putting the chamber on a hot-plate, I think, and putting a thermometer in the chamber. I would tend to do this with an Arduino.

A second question is: can "pulsed" vacuum drying and/or heating speed the trying time.

A second interesting experiment is: could we raise the pressue to 6 bar, and then exposively release it, to get a "puffing" effect of the 
greenwood, making it more porous. If so, we could then dry it more quickly, and it would like combust more quickly as well. NOTE: this should probably NOT be done in the vaccum chanmber, but could be done a strong vessel with a bicycle pump and a quick release mechanism.  The sample would PROBABLY have to be 
studied under an optical microscope after "puffing" --- I doubt there will be a change visible to the human eye. However, a microscopic change is 
all important for drying and combustion.

## Modularity

This system should be investigated as a series of modules with iterative functionality. For example, the O2 Concentration may not be possible,
but the vessel stove could still be incredibly effective without it.

## Some Arguments this is not Insane

If we imagine a "camping" experience, which is similar to what many people in the world live with on a daily basis, we can imagine a small solar panel
could be be used over the course of a day. By not having a battery of much size, we save a lot of expense. Throughout the day a modest amount of power
could be intelligently diverted to different parts of the system. For example, it may not be possible or necessary to run the O2 concentrator at the 
same time that the fuel is being dried. In fact, we can think of heating/running vacuum pump/running O2 system/running air compressor as separate activities that can all be performed at a leisurely manner as the available power allows.  Of course, this require a microcontroller with a modicum of programming sophistication; but this is now cheap to free.

The highest VO2 Max ever recorded has ben 94 L/min (male) and 77 L/min (female), both in Nordic skiers. A SMALL fire will consume more oxygen than that! A typical portable O2 concentrator that costs US$1000 produces 6L/min. Therefore it seems crazy to try to use oxygen enrichment on a campfire.  However, we have all day to store up O2 in a pressurized tank; we may be able to store 100L under pressure quite easily in an hour.

We do not need 90% oxygen to have a startling effect on combustion. Air is about 21% O2 in general.  Doubling or tripling this may make a fire burn much hotter and faster. This is potentially a very good thing, because it may mean that little energy is wasted in the flue gasses. Also, a hotter fire will shed heat through radiation much more; if this radiant heat can be directed into the stovetop (this is not obvious), then we may have a very efficient system.

It is unquestionably the case that drying fuel is more efficient because one does not have to pay the heavy cost of the heat of vaporization of the contained water.

## Modeling

As always, I believe the best invention exists at the interplay between theory and practice. As mentioned above, some experiments must be performed
becasue theory simple can't predict what will happen. However, we certainly could build an effect model, perhaps using only a spreadsheet,
of the inputs and outputs of the system, and of course we should do this before investing in equipment.

## A Call to Action

This project, like most Public Invention projects, needs an Invention Coach to drive it to completion and volunteers to do the work. This is one of the more difficult projects that we have proposed. I leave you with a quote from Sir W. Lawrence Bragg:

> The chances of your success are zero, but the importance is infinite; therefore, I support you.

To discuss this further, contact Public Invention or Robert L. Read <read.robert@gmail.com>, <read.robert@pubinv.org>.


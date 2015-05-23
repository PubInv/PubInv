Last sprint, I successfully prepared for and participated in the Austin Mini Maker Faire. I staffed the booth, and
the two demo projects that I had significantly added to the do that Anjan already had.  This sprint, I am going back 
to what I consider to be true "invention".

## Themes

I would like to do some significant work on the creation of an inexpensive latching linear actuator.  This 
is a precursor to one of my oldest ideas the [Gluss Robot](https://github.com/PIFAH/PIFAH/blob/master/ideas/Project%20%2316:%20%22Gluss%22%2C%20A%20Robotic%20Truss.md).

I would also like to play around with the Ferrofluid that I got.  Finally, I would like to really do the mathematics 
for both the neo-natal incubator idea and the pyrolysis of biological waste idea.

## Stories

* Figure out if I can get the 1/4" x 1/2" magnets into a tube for making the actuator.
* Experiment with apply the current loop to these magnets---I believe we will get a strong push from them.
* Try to construct an initial prototype of the actuator using just a power supply.
* Construct a new MOSFET circuit (similar to old one) and see if I can drive it fro the Arduino to properly
move the actuator to a different state.
* See if I can order an H-Bridge that will allow me to reverse current flow in a way that will allow us to change
the actuator state in both directions.

As a matter of procedure, if I can get anything working I will create a new Repo for this project.

## Log

In the last two days, since Mini Make Faire, I worked on the actuator.

I build a coil and a set of magnets, placed in some foamcore.  I was able to get it to move.

I think worked much harder, and built a good plywood holder for 6 of the 1/4 x 1/2 magnets. I held these in place in polycarbonate taped together.

I tried it, and it didn't work.  That is, it twitched. It did not do what I need it to do: move to one of the "pole" positions based on the current.

I was quite surprised that the force was insufficient, although my coil has only 30 or 40 turns, and mow power supply cuts off at 5 amps. Nonetheless, it was a failure.

I am attempting to construct the magnetic actuator anew with a poster-board wrapper. Hopefully this will be both "slicker", having less friction, and will be lighter. It is possible this model will work.  It is possible that I will have to go back to the drawing boards.

![imag0170](https://cloud.githubusercontent.com/assets/5296671/7717488/d201cc4a-fe67-11e4-90d6-f607678fe7ea.jpg)

![imag0161](https://cloud.githubusercontent.com/assets/5296671/7717452/696c9f84-fe67-11e4-8cde-7c1b951a6d59.jpg)
![imag0163](https://cloud.githubusercontent.com/assets/5296671/7717454/6970313a-fe67-11e4-8d89-eb21bc71caf2.jpg)
![imag0165](https://cloud.githubusercontent.com/assets/5296671/7717456/6973fa86-fe67-11e4-8f9f-e538a7f1a327.jpg)
![imag0167](https://cloud.githubusercontent.com/assets/5296671/7717453/696f8140-fe67-11e4-9946-693e15722392.jpg)
![imag0169](https://cloud.githubusercontent.com/assets/5296671/7717455/6972f24e-fe67-11e4-8186-548a4fa34717.jpg)

## Wednesday

I learned that the tightness of the windings really matters.  I'm now getting a few ounces of force, I imagine.  I have a strange assymetry in the actuator I built that I can't explain.

I tried using an aluminum tube and it seemed very weak --- possibly the Krebbs effect at work.

I embedded two magnets in a wooden dowel.  When that is placed inside a PVC pipe with a coil around it, I am starting to see the kind of behavior I expect, though the weird assymetry persists.

I am very tempted to buy some better materials---I know that will make a difference, but it is also a delay and an expense.  I want to carry on with as many experiments as I can at present.

General lesson:  It is really hard to get a coil 3/4" wide to discrimnate a magnet only a 1/2" long.

I've got a bistable system, but it should have 3 or 4 poles (for 2 or 3 magnets), that is, 3 stable conditions.  In stead it seems to "wash out" in the middle.  it is as if the flux within the coil is swamped by the flux at either end.

## Wednesday Night

I am a fool, but I have done it! My expectations were wrong.  It is clear if now that if you build a "comb" with alternative North and South poles each one will represent a stable position (probably just on the opposite side of the charged coil.)  I can now, just by switching power, move randomly through 4 stable states with 5 magnets.
The motion is random now because I can't control which state it will move to when I switch current direction driving it out of the current state.  However, that can be fixed easily in the future.

I think this is a great success.  IF this can be tied into a frame that provides permanent magnet latching, and IF I can get an Arduino to successfully switch on and reverse power (such as with the MOSFET circuit I built earlier, then it seems that I might have actually created something useful: A cheap, long-through, multi-polar linear actuator.

Note: I messed up the spacing on the magnets in my actuator.  I may have to redo in order to get the latching to work properly. Ideally I would have better materials by that time.

## Friday Night

The two-dimensional attempt basically didn't move very well.

I switched back to a tubular approach, basically re-inventing the tubular linear motor.

This actually "worked" in that I could easily drive a 2" crest-to-crest change using the coil.  This is similar to a 
coil gun, with a permanent magnet in place.

![imag0171](https://cloud.githubusercontent.com/assets/5296671/7781700/d26dcf86-00b9-11e5-914c-325e6de70a12.jpg)

![imag0172](https://cloud.githubusercontent.com/assets/5296671/7781706/fe6990f2-00b9-11e5-8a02-22daf59d06fe.jpg)

![imag0173](https://cloud.githubusercontent.com/assets/5296671/7781699/d26bef86-00b9-11e5-8c47-92364ee8b9e8.jpg)

I have learned a lot this sprint, though perhaps that is only a sign of how ignorant I am.

Let me try to summarize:

* Magnetic field computations are actually quite difficult. Unlike electrostatic compuations, the "field" the field is modified by anything ferrous. It is in fact quite difficult to to analytically figure out the forces. Also, there is no good free online simulation!
* I believe it IS possible to build a repulsive system, but it is rather complicated. Naive approaches produce a "pinching" of attractive approaches.
* The tightness of the coil is really quite important.  A lot of flux is wasted if the coil is larger than necessary.
* My system provides no control --- I can change state but can't control direction. It is fairly obvious how to control it with a separate additional coils.
* The best way to really handle this is to have a microcontroller really understand the position of the shuttle. I don't know a good way to do this.
* This is obvious, but if you take iron it will move to a central position on the coil.
* Using my 8-volt system with a limited amperage, I can make a nail repulse a small magnet.  However, my home-made electronmagnes are in general not as powerful as the neodymium magnets.
* I CAN easily build a latching system with the permanent magnets.  It is interesting to imagine a latching system that cooperates with the electromagnetic motion.  However, I now believe this is a distraction---getting the driving working is hard enough, and we can latch with a solenoid mechanically to be stronger and cheaper (I think) than we can ever hope to be with this pure magnets.


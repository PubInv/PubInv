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

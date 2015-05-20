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

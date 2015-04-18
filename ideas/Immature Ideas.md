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

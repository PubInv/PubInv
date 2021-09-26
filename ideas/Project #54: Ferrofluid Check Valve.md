# Passive Ferrofluid Check Valve

Ferrofluid has been used in a variety of micro-pumping and cooling applications, often associated with the idea of a "lab-on-chip". A number of active valves
have been developed. Because a pump knows its pumping state, active valves are sufficient to build small pumps.

However, it would be elegant to have a ferrofluid check valve of one-way valve that was completely passive, using permanent magnets with no electricity of moving
parts beside the ferrofluid itself.

I have racked my brains over this problem, and believe I have now found solutions (that have many limitations.) These are captured in these diagrams:

![Improved Idea for a ferrofluid check valve](https://user-images.githubusercontent.com/5296671/97095340-bd44c800-1623-11eb-93ec-d3c83e14aea4.png)


![Idea for a ferrofluid check valve (1)](https://user-images.githubusercontent.com/5296671/97095342-bfa72200-1623-11eb-91e1-c556253ef4a1.png)

In these system the idea is that a ferrfluid plug or bolus of area/volume A is in the center of magetic field. Then pressure differences push the bolus
eastward for westward. I believe by making the shape of the containing walls assymetric as indicated, we can make a fundamentally assymetric valve.
That is, one that allows the passage of air (or some other fluid immiscible with the ferrofluid) at a pressure which is different in the eastward direction than in the westward direction.

A perfect check valve would have zero cracking pressure in one direction and infinite cracking pressure in the other direction; this approach 
would certainly not acheive that. In fact it is rather difficult to build a ferrofluid seal or valve that can withstand more than 1 psi. Nonetheless, having a theoretical passive check valve would be an excellent step.

In order to work on this, I would probably:
1. Think about it theoretically more.
2. See if it could be analyzed with a finite element simulation.
3. Construct it a lasercutter or 3D printer out of semitranslucent materials and then use off-the-shelf ferrofluid and neodymium magnets to test it.

This depends on magentic flux gradients, which I think could be approximated with simple magnets; but that could be a weak point in theory.

If anyone wants to try making this, or discuss it, please contact me.

Our current work can be found here: https://github.com/PubInv/ferrofluidcheckvalve


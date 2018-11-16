# Rapid coliform presence/absence test

One of the means of determining drinking water safety is to perform a coliform presene/absence test such as those made by
[Hach](https://www.hach.com/presence-absence-test-pk-12/product-downloads?id=7640249610) or 
[IDEXX](https://www.idexx.com/en/water/water-products-services/colilert/).

These methods require incubation at a certain temperature an produce a color change in the presence of the organism.
Generally they require 24 hours or 48 hours.

It seems possible to produce a rapid test by building a machine that takes the place of the human eye that tests
the transmisssivity of a certain color, perhaps through a large linear quanity of the material. In theory 
this might detect a color change more rapidly than 24 hours.

For example, suppose that we could build a waveguide for water, consisting of a plastic tube with an index 
of refraction less than water. (The only plastic I know of that has this property is Teflon AF, made by DuPont,
which can [specifically](http://www.biogeneral.com/teflon-af/) be used to make a light wave guide.) The tube, when filled with water, would resemble a glass optcal fiber.
Light shined into one end would be totally internally reflected.

If we made a helical coil, we could easily produce several meters of light path in a compact space, still
containing 100 ml of water, the normal test sample size.

Then, the machine could, wich some sensitivity, report a graph of tranmissivity over time, using a simple LED 
and a photodiode.

The increase light path would multiply the sensitivy to transmissivity changes into a range detectable by 
a normal analog-to-digital converter, so long as the decreased trasmissivity was due solely to reaction of the 
reagent with the bacterial byprodut (if the water were very turbid, transmissivity might be so low this would not be possible.)

The result might be the ability to perform this test in a much lower time than 24 hours.

This would be a great boon in emergency situations. You could essentially test a an unkown source of water for 
fecal contamination indicator organisms in, for example, 30 minutes, to rapidly determine safety.


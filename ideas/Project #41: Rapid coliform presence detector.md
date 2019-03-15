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

![rapid detection of colorimetric change in water](https://user-images.githubusercontent.com/5296671/48650617-994ec580-e9bc-11e8-870c-d317e262a797.png)

Then, the machine could, wich some sensitivity, report a graph of tranmissivity over time, using a simple LED 
and a photodiode.

In theory, it might be possible to detect changes in the color in a rapid period of time.

The increase light path would multiply the sensitivy to transmissivity changes into a range detectable by 
a normal analog-to-digital converter, so long as the decreased trasmissivity was due solely to reaction of the 
reagent with the bacterial byprodut (if the water were very turbid, transmissivity might be so low this would not be possible.)

The result might be the ability to perform this test in a much lower time than 24 hours.

This would be a great boon in emergency situations. You could essentially test a an unkown source of water for 
fecal contamination indicator organisms in, for example, 30 minutes, to rapidly determine safety.

An improvement would be to use the same LED and the same photodiode for measuring both the control and the sample. However, we sould then need some sort of switch to shut off light to one of the tubes. One can imagine a mechanical switch of 
physical device in an air gap; some sort of Faraday effect with polarization might be possible but is probably not worth it.

# Update: Test of Light Guide

In February of 2019, we filled a teflon tube with water and attempted to use it as a light guide. At the scale of a meter, it appeared to fail completely. On the other, as would be theoretically predicted, when the tube was filled with nearly pure Ethanl (5% water), it worked as expected, sending all most all of the entering light to the exit end.
The index of refaction of Ethanol is much higher than the index of refraction of water.


# Understanding colorimetric changes

Here is the description of [Petfilim Chemistry](https://www.3m.com/3M/en_US/company-us/all-3m-products/~/ECOLICT-3M-Petrifilm-E-coli-Coliform-Count-Plates/?N=5002385+3293785155&rt=rud):

>The 3M Petrifilm E. coli/Coliform Count Plate is a sample-ready-culture-medium system which contains Violet Red Bile (VRB) >nutrients, a cold-water-soluble gelling agent, an indicator of glucuronidase activity (BCIG), and a tetrazolium indicator >that facilitates colony enumeration in food and beverage samples.

Violet Red Bile (VRB) is an [interesting chemical](https://catalog.hardydiagnostics.com/cp_prod/Content/hugo/VioletRedBileAgar.htm):

>Violet Red Bile Agar is a selective medium used to detect and enumerate lactose-fermenting coliform microorganisms. The medium is recommended for use in the microbiological analysis of milk and other dairy products, and for use in the examination of water. (1,2)

>The medium contains bile salts and crystal violet which serve as inhibitory agents toward some gram-positive microorganisms, especially staphylococci. Neutral red is employed as the pH indicator.

>Lactose-fermenting microorganisms produce pink to red colonies that are generally surrounded by a reddish zone of precipitated bile. Non-lactose-fermenting microorganisms result in colorless colonies.

Note: [E. coli](https://en.wikipedia.org/wiki/Escherichia_coli) is a Gram-negative facultative anearobic bacteria.


This is a description of [BCIG](https://foodsafety.neogen.com/en/dc-medium-bcig): 

>DC Medium with BCIG is used in the chromogenic differentiation of E. coli from other coliforms in water samples using the membrane filtration method in a laboratory setting. DC Medium with BCIG is not intended for use in the diagnosis of disease or other conditions in humans.

>DC (Differential Coliform) Medium with BCIG is a selective and differential medium for the presumptive identification of E. coli. This medium is enhanced by the addition of a chromogenic agent, BCIG, 5-bromo-4-chloro-3-indolyl-β-D-glucuronide to detect glucuronidase activity. The presence of the enzyme β-D-glucuronidase differentiates most E. coli spp. from other coliforms, and is the same enzyme used in the MUG reaction. BCIG reacts slightly differently, and when released into the medium is insoluble, accumulating within the cell, imparting a blue to purple color to presumptive E. coli colonies.


>Formula	Liter
>Lactose	10 g
>Tryptose	10 g
>Yeast Extract	3 g
>Sodium Chloride	5 g
>Proteose Peptone	5 g
>Bile Salts	1.5 g
>BCIG	0.2 g
>Neutral Red	0.08 g
>Agar	15 g








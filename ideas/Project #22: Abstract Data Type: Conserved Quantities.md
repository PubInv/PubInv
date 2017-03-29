# Motivation

In physics, we have conservation of energy and momentum.  In chemistry, we have the conversation of elements which
allows the balancing of equations.  In bookkeping we have the balance of debits and credits.  Although all
general purpose programming languages allow the construction of abstract data types (ADTs) that represent
these laws of conservation, there are rather rarely used.  They would seem, however, to offer the great 
benefit of reducing errors and clarifying programming.

For example, if you have variable that represent the quantities of chemicals that are the complete input and output to checmical (non-nuclear) process, it is clear that an ADT that guaranteed tha each operation conserved the amounts
of elements in the amounts of elements out would appear to reduce a certain kind of error.  Indeed, strong typing
in general is valuable for reducing such errors.  This would simply be an extension of that.

Additionally, one often sees [Sankey](http://en.wikipedia.org/wiki/Sankey_diagram) diagrams that attempt to visualize a complex process that shows inputs and outputs 
and their quantities represented visually.  As an example in sanitations is the [SFD](http://www.susana.org/en/sfd).
Another [example](http://www.energyvanguard.com/blog-building-science-HERS-BPI/bid/71262/Total-Energy-Use-Down-in-US-Wind-Solar-Up)
balances "electricity in" with "electricity out".

Mike Bostoc and Tom Counsell have built some awesome D3 code for making such diagrams.  However, my initial read 
of https://github.com/tamc/sankey suggests that it uses explicit (and absolute) quanities for the inputs and outputs
to each process, and then does the topological sorting and layout relaxing automatically.

If we know, instad, that we had a process like combustion that produced CO2, CO, and H2O from an input of O2 and
hydrocarbons, we could represent it as a balance and a set of percentages rather than as a absolute numbers.  Such
a system could easily sit "on top" of thie Sankey diagrams and produce the explicit inputs and outputs to be 
visualized.

Possibly this would be a valuable visualizaiton tool.

## Other examples

Bookkeeping.
Conservation of Energy.
Conservation of Momentum.
Invariants in loops.

## Noetherian Mathematics

I don't really understand it, but it is rumored that Emmy Noether as related symmetries to conservation laws.  This seeems deeply related.  What is the symmetry of bookkeeping?



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #22: Abstract Data Type: Conserved Quantities</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

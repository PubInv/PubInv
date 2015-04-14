# Motivation

In physics, we have conservation of energy and momentum.  In chemistry, we have the conversation of elements which
allows the balancing of equations.  In bookkeping we have the balance of debits and credits.  Although all
general purpose programming languages allow the construction of abstract data types (ADTs) that represent
these laws of conservation, there are rather rarely used.  They would seem, however, to offer the great 
benefit of reducing erros and clarifying programming.

Additionally, one often sees [Sankey](http://en.wikipedia.org/wiki/Sankey_diagram) diagrams that attempt to visualize a complex process that shows inputs and outputs 
and their quantities represented visually.  As an example in sanitations is the [SFD](http://www.susana.org/en/sfd).
Another [example](http://www.energyvanguard.com/blog-building-science-HERS-BPI/bid/71262/Total-Energy-Use-Down-in-US-Wind-Solar-Up)
balances "electricity in" with "electricity out".

Mike Bostoc Tom Counsell have built some awesome D3 code for making such diagrams.  However, my initial read 
of https://github.com/tamc/sankey suggests that it uses explicit (and absolute) quanities for the inputs and outputs
to each process, and then does the topological sorting and layout relaxing automatically.

If we know, instad, that we had a process like combustion that produced CO2, CO, and H2O from an input of O2 and
hydrocarbons, we could represent it as a balance and a set of percentages rather than as a absolute numbers.  Such
a system could easily sit "on top" of thie Sankey diagrams and produce the explicit inputs and outputs to be 
visualized.

Possibly this would be a valuable visualizaiton tool.

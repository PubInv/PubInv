# Oracular graph paper

There are different models of computation.  A variant of these is Compass and Straightedge construction, which
counts operations but is not generally a part of Theory of Computation as defined by textbooks.  If we think if this as a 
model of computation (I don't know to what extent that has been done), we can ask the normal questions
of computation complexity theory. Certainly the class "Constructable" exists within this space.

However, perhaps we can enrich the space by imagining "oracular" graph paper. Imagine that the paper upon which 
we draw with a compass and straightedge can perform a single operation which we do not know how to implement today.
It is thus an analog computer with an "oracle".  The "oracle" in this case answers the falling question:
given a semiplane and a point, does the point fall within the semiplane or not?  More colloquially, given a line and 
point, which side of the line does the point fall on?

This allows you to solve problems which cannot be solved using a standard Church-Turing computer, at least in 
the same time.  For example, because square roots are constructable, you can add one million roots together and 
compare them to a number in O(n) operations.  Yet this cannot be done in that time with an arbitrary number 
with a Church-Turing computer --- or at least, you certainly have have to stand on your head to do it. The 
complexity of this problem seems to depend both on the size of the input and the precision that you require.  Perhaps
it would more vivid to consider the space complexity of this problem: It is hard to imagine taking the sum of the 
square roots of one million integers that does not somehow retain all one million integers in space. It is hard
to imagine the one million boiling down to a smaller number.  Of course, you CAN boil one million rational numbers
down to contstant space quite easily---that is almost the definition of a rational number. Our oracular graph 
paper lets you boil one million square roots down to a single point "in space".

This complexity is interesting (to me) because it seems like this is an "almost implementable" oracle.  Analog computers have been
completely eclipsed by digital computers. However, there is a sense in which a compass and straight-edge can 
construct something that a digital computer has trouble with: computing a square root.  The digital computer of 
course can do this easily to any arbitrary precision.  The compass-and-graph paper idea does it in a single operation---
but only if you have ideal paper and an ideal compass and an ideal pencil.  Nonetheless we can imagine, perhaps
with lasers, or some other physcial system, that precisely placing points in space is not quite so absurd as
the other oracles that are used in for example the complexity theory of NP-hard problems, where those 
absurd oracles have proved very useful.

I conjecture that if we had this magic graph paper, there would be problems that could be solved in lower complexity
with it than with a Church-Turing computer, but that the graph paper is not so strong as to make make complexity 
hierarchy it generates collapse.  For example, since you can only one inequality question at a time, you cannot 
answer the question: is e + pi rational? in any obvious way using this graph paper.  You cannot instantly get 
infinite information out of the graph paper. You cannot compute the 10,000th digit of the sum of a million square 
roots in much less than 10,000 operations.

(Note: The graph paper does not come equipped with a grid, but you an easily add one.  So you can ask if a point
falls in a given square of your graph paper easily.  Then you can subdivide that square, etc. So the graph paper
allows you to obtain arbitrary precision for points, but this costs you the price of operations. The pencil, 
straightedge and compass that comes with the graph paper, however, are ideal: the pencil draws lines of infinitesimal
width, the straightedge is perfectly straight, and the compass measures distances perfectly and never slips.)

I'm not sure how to formalize this.  Do the drawn objects represent the space complexity of the problem? Are you 
allowed to erase objects, thereby freeing memory? 

What is the value of this supposed complexity model (and supposed hierarchy) related to the normal theory of computation?
Well, suppose there are two problems in the same complexity class in a Church-Turing model, but they have very different
complexity classes in the magic graph paper model. This would seem to give us some insight into the problems which
we can perhaps exploit to improve alogirhtms in the Church Turing model.

This seems a bit far-fetched, but when I read the large number of mathematical papers devoted to relatively specialized 
subjects, it seems at least interesting to investigate this.



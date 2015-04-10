So, imagine a horizontal piston and cylinder.  It pushes a pin in a slot.  The slot is defined by a curve C.

C(x) : has a domain of 0 .. T

T is the throw of the piston.

Piston has Head H and Area A.

V(x) = (H+x)*A.

For adiabatic gas:



Where Gamma is possible 5/3 or 7/5 depending on the gas.

The system of the curve must be such that the force exerted by the piston is always at least the force exerted by the mass to be raised, m.

Then we can write the constraint:

P(X) = constant / [(H+x)*a]^gamma.

Fh(x) = P(X)*A.

We relate the horizontal force to the Vertical force by:
Fh(x) = C(x)/dx * Fv(X),  where C(x)/dx is the slope at x, as rise over run.

So, by algebra:

(1)   P(x) * A = C(x)/dx * Fv(x)

However, we assert that for the machine to move,
C(x)/dx * Fv(x) >= C(x)/dx * M, where M is a constant.

So: 
[2] K * [(H+x)*A]^-gamma = >C(x)/dx * M

And M can be divided out, to create an expression that can be anti-differentiated to obtain:

C(x) = a constant + [K*A^(1-gamma)/M] * [ (H+x)^(1-gamma) / (1 - gamma)]

And so we have a graphable, close form expression for C.

C(x)/dx is the slope of C at point x.

Now, what is the Curve C(x) that maximizes work?  Well, to find this, we want to find compute the slope that satisfies [1], and then recurve the curve by integrating.

So, if we write all of this up, we have found the maximum way to extract work from a single compression cycle of a gas.  It would be interesting to compare this to other ways to extract work, such as crank-slider, offset crank-sliker, crank-scotch yoke.

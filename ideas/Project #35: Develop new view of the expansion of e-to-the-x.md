# Develop a new way of thinking about the expansion of e. (and sin, and cos)

This is a an admittedly half-baked idea.  My knowledge of analysis is woefully incomplete, something I am attempting to remedy.

Nonetheless, as a "public inventor", I work in the light, even the light shows how silly I am.
 
Consider the Taylor series expansion of [sin x](https://en.wikipedia.org/wiki/Taylor_series):

Sigma (x = 0 -> infinity)  -1^n * x^(2n+1)/(2n+1)!

Now speaking only for myself this is deeply weird to think that no matter what x we put in, this summation stays in the
interval [-1,1].  To a mathematician, this might not be weird, but think about this as a computer scientist.
We know it sort of make sense that x from 0 to 2 * pi is going to beheave somewhat reasonably.

But consider if we put in x of "100". The first terms in this expansion are GIGANTIC. In fact if you plot them
they rise and rise up to a maximum.  The values are alternately negative, which is what keeps the result from being 
huge.  If we look at the "envelope" of both the positive and negative values it will have a pronounced bulge 
which increase as x increases. The values get huge, yet always seem to cancel out.

I'm told the proof that this expansion is periodic is tricky, and I believe it --- it seems crazy that it can be.

Now thinking as a computer programmer rather than a mathematician, doesn't this mean that we are representing 
our series incorrectly?  Doesn't it make sense to recast the series in terms of where the maximum value is?

If we were calculating this by hand, we would not start at the 0 term---we would start at the maximum value,
and then adjust moving to the left and right of this value.

Basically, the fact that x^n/n! grows with x up to a point and then diminishes suggests that they're may 
be some valuable way of looking at the summation differently.  (I know this is vague statement.)

The maximum of the x^n/n! tends to occur near x = n. As x increases beyond n, each increment of n decreases our running value.
I propose that we find a formal expression for the maximum, and construct a series where that is the first term
in the series.  In order to make this symmetric about this value, we will have to manipulate the tail of the series,
since the series starts at n = 0, which is in fact assymmetric.  Possibly through some manipulation we can find
a manipulation which is symmetric about the max point.

Note: I have proven the maximum magnitude occurs when n = floor(x).

I believe an interesting algorithmic approach would be to compute "compensatory pairs".  The idea is to take the maximum
and the next term, which are of alternate sign. Add them together using a rational arithmetic approach. These two
terms form a fraction like (1 - x) * x^n / (j+1)!. If fully evalutated, this term is of relatively low magnitude, because
it is of two terms that are close to canceling in a certain sense. Then add to this the same calculation for the pair
to the left, then the same calculation for the pair to the right.  After you get back to zero, start taking pairs
only incrasing magnitude.  In a certain sense, this approach keeps the values relatively small. After performing 
numerator addition (subtraction) one can then look for factors in the numerator and denominator which cancel at 
each step, greatly reducing overall magnitude, potentiall.  The absolute value converges to the value of the series
rather quickly, in a limited sense.  Note this can be used to compute e^x as well (though the terms are all positive
in that case, you are at least looking for the largest terms first.

Note: It may also be interesting to investigate at what value of n x^n/n! becomes less than 1.0, or 0.1, etc. and when
the summation of all terms n > this value becomes less than 1.0 and 0.1 and other fences. Knowing this would allow
you to know how many terms are needed to compute a given accuracy of e^x.  This would allow you to perform all addtion
ahead of time, forming a single rational fraction, and then look for simplications so that factoring would be 
performed only at the last step.  The result would be a completely rational, unrdounded lower bound on e^x. So in a since
know where to partition the series starts to become very valuable.  If you know that there was less than one 
millionth remainin in the terms x^n/n! where n was greater than 352, then one could add together the first 351 terms
with a certain security.
would let you estimate how many such terms would have to be added to obtain a given precision.

Since x^n/n! decreases rapidly when x > 2n, I think it should be quite possible to put effective bounds on the remainder of the
series.

After studying a bit more how the power series for sine is developed from Taylor's Theorem, I think I have been a little
stupid---since the power series is developed at SIN(0), of course it converges more slowly at SIN(X) as X is far from zero,
and in a sense this is "just" the behavior of a Taylor's series approximation.

However, in my mind it does still raise certain questions:  Can we develop a different expansion for sine than one at zero?
For example, can we use 45 degree angle points (this depends on the knowability of the nth derivative at those points.)

However, the issue still stands in the computation of e^x or in a Taylor series in general.  Is it not better as a 
computational strategy to compute the terms in order of their size? (and, as we can see, if x >> 0, the first term is not
the largest in the e^x expansion.)

Would it be possible to choose a Taylor expansion around a different point that would produce a power series that would be
more efficient for the computation of the sin(x) (or even e^x)?

I've been trying to study this and I clearly I have been confused but I remained astounded that the Taylor expansion of SINE 
about 0 is A) Periodic, B) Bounded between [-1.0,1.0], C) capable of resolving such gigantic terms down to such small numbers.

Perhaps this is just my own stupidity, but I think it must be worth deeper consideration. There must be some other way 
of loosing at the summation of the series which explicates these bizarre features.

For example, what if we took some other function, such as sine(x^1.1), or sine^3(x). Can we produce the series of these at all?
The trick of eliminationg the nth derivative will clearly not work. 

How is it that this series has (in some sense) a period of 2PI? How can we deduce this from the series? 







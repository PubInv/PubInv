# Permanent Memory in Programming (Forgetting Should Be Explicit)

Suspect disbelief for a moment and imagine a programming language in which nothing was ever forgotten unless a specific command to forget was executed.
There may be an extant name for this, but I am unaware of it. We could call it "write-once memory" or "explicit forgetting".

By this I mean that when we execute a statement like:

> a = a + b

We record the value of *a* as a new value, but we retain the old state/context, so that we could build a debugging tool that would let us explicit step backward.
We insist that we retain all programming state so that we could explicit step backwards until the very beginning of the program, performing each
step backward in O(1) time.

# Infinite Regressive Debugging

The first implication of this is that we could always debug backwards in time.
However, we could write a much more powerful debugging tool. For example, we could compute against the program trace/execution history
very power *post hoc* assertion checking, such as "did the variable *a* ever have a negative value?"
Often, a programmer in the act of debugging does know what questions to ask until the execution has been studied. In that 
sense, debugging is a conversation between the programmer and the execution.
The programmer asks a question, the execution answers.
However, the programmer normally has to *rerun* the exectuion to answer this question.
In the case of intermittent bugs, duplicating the bug may be quite difficult, but if we stored the entire execution history,
this would not be a problem.

# More Effective Unit Testing

Today the modern style of programming is to use automated unit tests, which typically immediately stop execution when a computed assertion fails.
The programmer then begings debugging, usually with a "code-eval-test" style, but sometimes with an automatic debugger.
However, in not case does a modern system (AFAIK) really do what would be optimal: preserve the entire execution history to allow it to be fully 
examined. Such a system would allow more effective test driven development, or more effective testing after the fact.

# On Implementation

It might at first appear that this would be horribly slow. This however, is really the case so long as you have enough memory.
You would have to preserve every stack frame, for example, but that costs nothing in terms of time. You would have to 
have spaces with names for every variable version, but that also costs nothing in terms of time.

If the implementation were a lambda-calculus like system (perhaps Haskell counts), one would not store variables
but would store entire expressions before beta-reduction, but the priciple is exactly the same.

# On Editing Programs

Intriguingly, such a system could allow a program execution to be mutated in accord with a change of input.
For example, imagine a program to add 100 numbers.
Now, suppose that one of the numbers changes, (we know which one) and that we want to recompute the sum.
The compiler/interpreter could "flow" this change through the progam execution to rapidly obtain the 
new result. 

In this case, the programmer could write a special routine to handle a change. But that is a far cry
from the compiler doing it automatically for them.

We could even imagine a change to the program itself (not the input) being effectively applied to the program
execution. We could in some cases imagine a "change calculus" that takes program changes and executions and 
computes correct new computations based on the change.  This could in some cases be extraordinarly efficient.

# On Explicit Forgetting

It may even be the case that this may save power at a low level because it is erasing (returning to an ordered state)
which costs power at the theoretical bit level, not computation, which increases disorder.
However, we can easily imagine a programming langauge in with a statement like:

> x = current_execution()

(reminiscent of the famous *call/cc* function of list) that makes the current execution a reflexive and processable 
object. Such an execution can be stored, changed, debugged, analyzed, and restarted!

Similarly, we could have a command like:

> forget_execution()

which was an explicit indication to the compiler that it was legal to "forget" part of the execution.
Whether this would be interpreted locally or globally is unclear to me now---both are possible.
You could explicitly forget the internals of a function if you knew it could be re-executed efficiently
by starting over with known parameters (this would sometimes be intractable.)

# How to Investigate

This idea needs to be researched with Google Scholar to see if it is known (I have not done this.)
If it is a new idea, it would be interesting to hack an existing language to try to support it.
This could be done in Python, Node, Common LISP, etc.

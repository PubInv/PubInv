# Computation Theory based on Progressive Refinement

Today, the Theory of Computation is based on the formalism of input strings. Sets of strings are called languages, and 
the theory of computation formalizes problems as languages and the recognition or acceptance of languages. 
This sounds a little weird if you have not been introduced to it.  See for example Sipser as a reference.

This is a beautiful and power theory; it ties computer engineering to fundamental mathematics and even physics. 

But it has a blind spot: not every problem can be easily expressed as strings.  (I know that sounds naive, but bear
with me---I do have a PhD in this subject.)

For example, if we force a physical measurement or the computation of an irrational into a string, we tend to force
into into an approximation. In a sense we turn a blind eye to the real computation, because we have such a wonderful
theory of computation for dealing with something a little simpler.

I propose that we consider, perhaps just as a playful exercise, redeveloping the formalization of finite automata,
pushdown automata, and Turing Machines and lambda calculus in terms of progressive refinement of the inputs.

The "input" is not a string.  The input is a process which gives you greater and greater precision over time.

One could explore what is computable, but even better what is efficiently computable (what is known as complexity theory)
based on this approach.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #7: Color-block-based Writing System</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

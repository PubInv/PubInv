# Polytext

The idea of a text was once two-dimensional. Pictograms, glyphs, letters, drawings, and decorations coexisted on a surface.
Movable type gave words a formal value that allowed a text to exist abstractly, more divorced from the page on which it was written,
moving it from a 2-dimentional surface into an abstract space.

There have always been footnotes, but hypertext quickened the footnotes into a live structure.

Recent innovation such as "rap genius" have turned texts into multi-commented documents.

It is time for us to go further and to define a true polytext.

This idea is not fully developed; please bear with me as I put down these half-baked ideas. These ideas owe a lot to 
Ted Nelson's ideas of transclusion. However, it may differ slighlty in not necessarily producing an single integrated
text as a result (thought that is clearly possible.)

# Comment Texts

I cannot yet conceive of two texts which are truly peers. It is easier to imagine one text to be an *original*, and 
other texts *derived* texts which are only meaninful in connection to the original.

However, we already have a model of multiple derived texts. If the original is immutable, it is easy to 
connect to the derived text to the original. If, however, the original is allowed to evolve over time,
the connection of the derived text to the original may be lost. I suspect we could, however, make a very
powerful pattern matching system to create anchor points in the original text which will remain easily identifiable
even when the original text is wildly rearranged. This has show itself to be possible with *diff* and *patch* at
the level of lines. AFAIK, nobody has extended the *diff/patch* system to work inside lines. It would be 
extremely valuable to do so, and that would be a nice, separate work.

The comment text may then be thought not as a sequence but as a collection of comments, each of which 
identifies a pattern which specificies one or more anchor points in the original text and then the modifying text.

# On Rich, Literate Programs

One of the most important forms of text the computer program. In the case of the computer program,
having a large number of derived texts that could be "turned on and off" would be extraordinarly valuable.
We can imagine a system in which the compiler operates on not only the original text, but the text
computed as the orginal plus dervied texts. The derived texts could then be thought of as "channels" which
could be enacted. A programmer can instantly recognize the value in:
1. Adding assertions in a derived text. These could be configured to be executed or not at will.
2. Adding comments in a dervied text.
3. Adding debugging statements.
4. Adding logging statements.
The power of controlling this alone would be enough to justify working on this idea.

Modern programming is done with Integrated Development Environments or extremely programmable
editors such Emacs. Making these editors aware of the polytext would be extremely useful.
One of the advantages of this is that would NOT be specific to a programming language, but would
be the same whether one was working in Python, C, Node.js, or Haskell, and would also be the 
same if one was working in TeX or commenting on plain old text (ASCII) file.

Programs change; sovling the problem of attaching anchor points which survived most
edits would be a major issue.

# On Poetry

A similar richness could apply literary criticism. If we imagine the original text as 
a poem, we could add:
1. Analysis of scansion
2. Historyical comment (what did this word mean to Shelley?)
3. Translation into other languages
4. Explanation of adumbration
5. Personal impact ("This line reminds me of my dear mother...")

There could be many derived texts, even of the scansion, of a famous poem.

# On Redlining

Microsoft Word offers power "redlining" which is in particular used by legal experts and 
attorneys when attempting to make precise language for legal documents. A polytext system
could be potentially create better redlining than we have today.

# On Functional Texts

In general, we think can think of a comment text as set of constant comments on the original. That is,
the comment text is a text, and not a function. However, we could think of a comment as a computable function
of the original text. That is, we specifiy the comment text as commenting on a part of the original that
begins at point A and ends at point B (perhaps a few words within the same line.) Instead of merely 
being words, the comment text could be generalized to be a computer program that takes as input those 
words. The output of this program would again be a text (or, mindbendingly, a program).
This would create a very powerful system for commenting. For example, the program could translate the words
into a different language, or translate a mathematical equation into LaTeX for typesetting, or fill in 
an anchor with data values, like a form letter.  The text would then become an executable object which
would produce a new text. This would be more powerful if the original text could survive edits.

# On the Production of an Output Text

A fundemantal operation is to take an original text and one or more derived text and compute 
from them a single, integrated text. This is called transclusion.

In general, however, "inclusion" need not be the main point. The derived text may specify
actual changes (not mere inclusions), and may be interpreted to modify the original text,
or to add links to it, or both. 

There are so many interesting things that could be done with this idea that selecting
the simplest and easiest to implement first is probably a matter of great importance.

# How to Perform this Work

Although much conceptual work needs to be done, it is clear that this work, like the extraordinarily
impactful *diff/patch* pair, needs the development of a set of tools and a set of standards. However,
it probably needs nothing more than a simple set of filters (in the Unix since of that word). That is
this work can be done as nearly pure algorithmic programs that operate at the command line. 
Integration with a browser, which would be extremely powerful, could be done later.

# Distinct Parts of the Project

1. Pattern-matching anchors that operate within lines
2. A standard for defining computational operations
3. A standard for naming texts such that a derived text could be clearly associated with an original text.

# References

This system performs scansion of Engligh poetry. It could be useful for as a source of child texts for testing.
1. https://yadda.icm.edu.pl/baztech/element/bwmeta1.element.baztech-ca6efb02-dfd3-498a-b7f4-ca33197d8ea0

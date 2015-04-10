# Lovecraft: The Programming Language

## Goals

I really want to have a programming system (it really could work with any language) that allows infinite debugging
back to the beginning of the computation.

I believe this is completely possible by "meldling" the concepts of a source control versioning system, a programming
system, and database.

That is, we can build a system where every change of state (modification of a variable) is a revision, and all state
is stored in the database.  There will no longer be a clear distinction between the persistent store and the dynamic state.

We should be able to rewind and restart the computation at ANY point.

The source code itself must be considered a part of the data.  In this way, we can rationally make a change to the 
program (that is, fix a bug, for example) and STILL be able to debug back in time past this change (and run forward 
from that point as well.)

## Principles:

There is no distinction between compilation and execution.  All is compexion in the presence of more and more information.
* Compexion is controllable.
* There is no distinction between a program execution and a database.
* All state changes are the creation of new versions.
* All program edits are the creation of new versions.
* Synchronizing clocks is an intentional act.
There is a clear distinction between function execution and state change.
A clock synchronizes a collection of variables.


## Example:


## Guiding principle:

1) Any machine can be rolled back precisely and infinitely.
2) Machines are recursive.
3) Machiens have repls.

## Commands:

    (ANDASSIGN (VAR EXP)*)
    (ORASSIGN (VAR EXP)*)
    (COND VAR (TEST EXP)*)
    (WHILE VAR TEST EXP)
    (BOX VAR (TEST) PROGRAM)
    (MACHINE PROGRAM)
    (FREEZE MACHINE)
    (THAW MACHINE)
    (ADVISE MACHINE)
    (KILL MACHINE)
    (REWIND MACHINE VERSION)
    (CREATE VARIABLE)
    (READHISTORY VARIABLE)
    (DESTROY VARIABLE)
    (COMPILE CODE)
    (READ INPUT)
    (WRITE OUTPUT)
    (TAKE SNAPSHOT MACHINE)
    (DEBUG SNAPSHOT)
    (CREATE CAMERA)
    (SNAPSHOT CAMERA)
    (DEBUG MACHINE)

## Notes:
It should always be possible to create a new REPL on a machine.  You can always DEBUG a machine.  However, Debugging a machine may not give you vision into its sub-machines.

A Machine is not “IN” a state.  A Machine is “Past” or “Post” a state.

Making a distinction between INPUT and OUTPUT allows us to build clocks and cameras more efficiently.

Random Numbers are generated as INPUTS to machines that can be read any number of times.

In Lovecraft, a statement like “STOP WHEN X==4” is reasonable because we can control modifications to X in a reasonable way.

At this point I have not really clarified the difference between a clock and a camera.

Thoughts after isolation float on March 30th:

1)  We can map FILE to a type, therefore allow practical editing.  This is a necessary compromise.
2)  A MUDD in which players trade gold is a good test bed for this system.
3)  Pretend a hacker has done something naughty and trying to rewind is a good demo application.
4)  Build a version visualizer into the first example.


Note that [Arvados](https://arvados.org) has already done this: they are recording everything in Git.  We can imagine simply making a major improvement to Arvados to lower the cost of using for small computations.

## Difficulty

This is a borderline research project, so it has to be classed as fairly difficult.  However, I believe it will be easy
to storify, and to incrementally execute this project.  Of course, performance is likely to be an issue---but then,
isn't it always?

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #2: Lovecraft, The Programming Language</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.

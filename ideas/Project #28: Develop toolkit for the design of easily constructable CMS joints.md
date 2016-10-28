# Develop toolkit for the design of easily constructable CMS joints

## The CMS Joint

The CMS Joint invented by [Hamlin](https://www.google.com/patents/US5657584) is a great mechanical invention, particular
in the cotext of "ideal" trusses. By ideal, we mean trusses in which each member is aimed perfectly at the center of
each joint with a joint allowing rotation, thereby limiting developed stress and strain to purely compressive and tensile forces.

However, it is not too easy exactly how the maker with access to a laser cutter and 3D printer should go about
constructing such a joint. We note the extremely valuable websites such as [makeabox.io](http://makeabox.io/). This
websites makes it nearly trivial to produce a design which can be immediately cut out of plywood, plastic, or other
materials, using a laser cutter or CNC machine.  (I've personally done it.)

## Project

The idea of this project would be to produce a free usable tool that would be as convenient as "makeabox", but
for the purpose of creating the CMS joint components.  That is, basic parameters would be input, and output would
be laser-cuttable and/or 3D printable designs which could easily create the CMS joint. Note that Public Invention
has already produced a simlar project, [Coil Choice](http://pubinv.github.io/CoilChoice/).

## Anglular Limitations

An important aspect of the CMS joint is that it has a wide, but limited, range of spherical angular motion.
(As each such joint joins two members, this may be consider an planar angular range.) Therefore one of the
most useful aspects of this tool is to state the minimum and maximum angle for a give set of paramerts.
Gregory J. Hamlin and Arthur C. Sanderson's book,
[Tetrobot, A Modular Approach to Reconfigurable Parallel Robotics](https://play.google.com/store/search?c=books&q=TETROBOT),
provides, beginning on page 53, a mathematical description of these issues. The resulting equations are of
sufficient complexity that a spreadsheet-like ability to compute them quickly for a given set of parameters
would be very useful.


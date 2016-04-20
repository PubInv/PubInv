---
layout: post
title: Gluss Pusher Intro Video Script
---

<section class="content">
      <div class="jumbotron">
        <h1> Gluss Pusher Intro Video Script</h1>
      </div>

<h2>Audience</h2>

This video is primarily for the maker, inventor or engineer interested in 
robots or
mechatronics, alternative approaches to robotics, or even those
interested in kinetic sculpture or possibly cosplay.

<h2>Project</h2>

This is the introductory video for the a project I call the "Gluss
pusher". The world "gluss" is a portmanteau of "slug", "glass", and
"truss".  About 25 years ago I was carefully studying the way of
thinking popularized by Buckminter Fuller which he called
"synergetics". Synergetics argues that you should think primarily in
terms of triangles. Bucky created a number of omni-triangulated
structures, of which the geodesic dome is the most popular. However,
he also invented a space-filling truss known as the octet-truss, which
exploits the remarkable fact that you can create a repeatable slab out
of alternating octohedrons and tetrahedrons.  In the octet truss every
structure member is the same length.

I have always been fascinated with the idea that if we could make a
structural member that could change it's length, growing shorter or
longer on command, and if we could coordinate many members moving at
the same time, we could construct a machine, or robot, that would be
quite unlike existing robots that depend very heavily are wheels and
articulated joints. We could make a robot that "oozes" like a slug. We
could make a dancing truss.  Rather than simulating the human form, which is a
slightly arrogant thing to do, we could mimic worms, slugs, and the
human tongue. This seems both a humbler approach to robotics, and
would have the advantages of massive modularity and scalability. Such
robots would be made of "gluss" --- a truss that is not a crystal, but
rahter a glass.  You could join a 50-member gluss to 100 member gluss
and have a 150-member gluss.  I thus use the word "gluss" as the word
"clay" is used--as a substantive noun.

Such a flexible gluss would be able to do things that existing robots
find difficult:

* Climb over a building,
* Climb up a tree,
* Fold iteself into the bed of pickup truck,
* Tolerate the dysfunction of some fraction of members,
* Burrown throw earth like a worm,
* Swim in a variety of ways.

I hope this project creates a new subfield of endeavor that I
call "glussionics". I hope controlling a gluss will become and interesting of field of research. The difficult problem of programming a gluss to climb over a building appears to exist in the thin boundary between the impossible and the trivial. The impossible need not be attempted, and the trivial is a poor use of our precious time.

<h2>Existing Systems</h2>

I do not necessarily claim that this is a particularly novel
approach.  For example, NASA has constructed [robots](https://youtu.be/wR0AlIwEgSE) based on a
different principle, the principle of tensegrity, which was also
popularized by Buckminster Fuller. 

It is entirely possible to start constucting a gluss robot from
existing machines that you can purchase, which are generally called
Linear Actuators.  For example, the firm
[Phidgets](http://www.phidgets.com/products.php?category=39) sells or
resells a actuators starting at $70. Other firms make tubular linear
motors which are probably more expensive, since they require that you
ask for a quote.

I may purchase some of these devices to learn more about about
them. I believe these systems are generally good machines---perhaps
too good.  By
that I mean, they are too heavy, too expensive, and too forceful, and
too slow. 

What we, the hobbyists who would attempt to make gluss
robots really need, is something closer to a $10 or $20 price point to
make building a 100-member gluss reasonable.  Additionally, an
open-source hardware solution would allow us to experiment with
different designs.

I believe that if we can make it possible to build an interesting gluss for
less than $1000, we will be able to harness the tremendous creativity of the
make movement.  For example, 3D printing was first developed by Universities, but has exploeded in recent years as the price of a printer has gone down 
allowing a large number of creative people to experiment with 3D printing.

The Gluss Pusher projct is an attempt to make just that: an
open-source hardware and software, inexpensive, easy-to-control
structureal member that can change its length. This video is my
invitiation to you to join the team, if you are so inclined.

Do I believe that I can do a better job engineering such an actuator
than the firms that are already doing so? No, I do not. In the first
place, I am a computer scientist, and my understanding of electrical
engineering and physics is sketchy.

What we together can do
is explore an relatively unexplored part of the design spectrum---what
a cynic might call the "shabby" part of the design spectrum, where the
gluss pusher is less strong and possibly less precise than existing
designs. Nontheless, this part of the design spectrum may be very
valuable to makers.

<h2>Basic Idea</h2>

My basic approach so far has been to build a tubular linear stepper
motor that is as simple as possible.  The video below shows the
current prototype in operation:

<iframe width="560" height="315"
src="https://www.youtube.com/embed/o0czhRU1vQM" frameborder="0"
allowfullscreen></iframe>

I suspect you will get more from the video than a spoken explanation,
but let me try to explain it.

This is basically a tubular linear motor.  The pusher rod is an
acrylic rod. Into it are place 1/2" by 1/4" rare earth magnets which
can be obtained from Apex magnets for $10 for 10. The magnets are
carefully spaced exactly 1/2" inch apart in the rod, facing each other
in a repulsive way. That is, the North pole of magent faces the North
pole of the next magnet.  This produces a magnetic "comb" of
alternating polarity.

The motor itself is two coils of magnet wire spaced preciesly 1.5"
inches apart. When voltage is applied to one coil, it seeks a stable
position, in this case centered directly on top of a magnet. Two coils
are required to avoid dead spots.  An Arduino microcontroller is used
to control the application of an external voltage.  An external power
is required becase the coils draw a few amps at 5 volts, far more than
the Arduino can source.

Whenever a coil is centered, the other coil is not---and application
of voltage to the other coil will drive the the push rod left or right
relative to the coil bobbins. Thus moving is always applying energy to
alternating coils. The Arduino stores the state of which coil is centerred over a magnet, and which magnet it is over. 
The direction of the voltage to apply depends on
which direction you want to go. At present there is no ability to sense the state of the push
rod.  If you move the push rod by hand or if a force prevents it
moving, the Arduino program will do the wrong thing on its next
command.

A major goal of future work is to provide robust position sensing. We
need to be able to ask the microcontroller where the member is, and
determine when it is failing to accomplish our command to move to a
given position.

<h2>Driving Applications</h2>

Although there are a huge number of uses for a functional Gluss
Pusher, I have found that it often best to be driven by a specific
application even in attempting to develop something completely
general.

As Kent Beck taught me, I always try to do "the simplest thing that
could possibly work". The simplest actual use for a Gluss Pusher that
I can imagine (outside of some art project) is to create a triangle of
two gluss pushers and one fixed member to make a planar robot.

This could be hung on a wall or laid on a plane to do the same sort of
position that is done by laser cutters, plotters, and and 3-D printers
if you take out the third dimesion.  Those systems almost always use
belt-and-pully systems for precise position, and that is almost
certainly better---if you you can fit your work object into the
bed. The 2-member planar robot could concievably be used to paint a
wall that is already in place. I of course don't expect the initial
prototypes to be forceful enough and precise enough to really do
something like that well, but progress is made by taking baby steps as
fast as you can toward the goal.

<h2>To Be Dones....</h2>

To that end, I'm sure if you have followed me this far, you are
probably thinking of a dozen or so improvements that can be
investigated right off the bat. Here are the ones that appeal to me
most:

* Make a 3-D printer design for the bobbin that holds the coils and sensors.
* Add Hall effect sensors to detect when we have failed to move
  correctly.
* Add color sensors that allow us to detect position from a cold start
  based on colors painted on the push rod.
* Construct an actuator shaft for the bobbin so that we really have a
structural member.
* A modular way to address many gluss members.

So my basic plan is to work on these things in an attempt to build the
2-member planar robot.

<h2>Multiple sizes </h2>

In addition to the "1/4" inch diamter magnet size, I have also build some working prototypes using 1/8" magnets.  One possibile advantage of the current 
linear motor approach is that it may be possible to make smaller actuators than can be made using rotary motors and lead screws at a low cost.

Even a very small, weak machine made from small gluss pushers would make a fun development platform so long as it was strong enough to move itself into programmable positions. Imagine a gluss composed of 200 members, each a mere 2" long, that could sit on your desk and quickly assume a menagerie of shapes.

<h2>Part of PubInv</h2>

The Gluss Pusher is one of several projects that I am undertaking as
part of my effort to create a charity or movement called "[Public
Invention For All Humanity (PubInv)](https://github.com/PubInv/PubInv)". As
such, as it obeys the principles of PubInv, which are:

* We will be completely transparent and open from the first.
* Everything we produce will be shared to everyone without exception.
* We will organize our work using an Agile methodology, whether our
  work is software, hardware, research, or education.

So for example, I will seek no patents on anything I develop as a part
of PubInv. All hardware designs will be licensed with a Creative
Commons Share Alike license, and all software will be licensed with
the Gnu Public License. If anybody attempts to patent anything
published here, I will fight them legally. However, I have no
objection to people making money from anything developed by PubInv so
long as they do not violate the licenses. I would view it as
acceptable if a firm started making a Gluss Pusher, so long as they
conform to the law, and I would consider it a great success if they
would conform to the spirit of creating and adding to free and
open-source designs.

<h2>About me</h2>

Am I qualified to run this project? Actually I am tortued by
self-doubt everyday. But let me tell you just my qualifications that
may make you want to join this project.

In the first place, I'm good at running teams and have been running
multiple software teams for a long time. I love working with beginners
and teaching people and am good at it. Although I am not much of an electrical engineer
at present, I have a PhD in computer scientist. I recently was a
Presidential Innovation Fellow, which led to work where I created a
team doing very innovative work for the Federal government, called 18F
Consulting. I co-created a foundation to support the Presidential
Innovation Fellows, and I hope that experience will help in the
creation of PubInv.

Finally, I am focusing on PubInv mostly full-time. I of course don't
get paid, but am volunteering my time. There are not many people who
have the good fortune and freedom to do something like that, and I'm
hoping to make the most of it, possibly with your help.

I suspect trying to run an open-source hardware project like this will
be harder than runnign an open-source software project, because the
number of people who have an interest, and the modest amount of money
needed to purchase tools and supplies, is much lower than people
capable of working on pure software projects. Nonetheless I feel
called to try this, and to expand the Free-and-open source mentality
to hardware projects, and even invention, as much as possible.


Obviously, people interested in physics, electronics, and robotics can
help this project.  However, I believe true creativity comes when
well-rounded teams are formed.  I would love to have an artist make
some conceptual sketches of big gluss robots, for example. An
entrepreneur might find a valuable use for glusses that we could aim
to fulfil. Writers and marketers could help me recruit people to this
project. So, if you have any interest or questions, please contact me
by email: <read.robert@gmail.com>
or visit our Github repositories, under the organization PubInv.



</section>

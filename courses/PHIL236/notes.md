<head>
<script type="text/javascript" charset="utf-8" 
src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML,
https://vincenttam.github.io/javascripts/MathJaxLocal.js"></script>
</head>

# Disclaimer

To students using these notes to catch up on missed material: these notes are not official  notes for the course, they are notes I use for myself to teach from and are not designed for students. They are in no way a substitute for the lectures.

# Euclidean Geometry

We'll begin our study of space by examining the oldest theory of space:
Euclid's Elements. A very old treatise on space, written around 300BC,
is, according to Bertrand Russell, one of the greatest book ever
written.[^1] Euclid's Elements is essentially a summary of the ancient
geometers' knowledge at this time --- few of the theorems found in the
Elements are actually due to Euclid. What is remarkable about the book,
however, is the way it is organized. Euclid reduced all of the notions
of geometry to a few basic notions---notions like point, line and
circle---and reduced all of the ancient geometers knowledge to five
basic postulates. By starting with these basic postulates, he was able
to reconstruct many complex theorems of geometry known to the geometers
of that time.

## The Primitives of Euclidean Geometry

Basic notions of Euclidean geometry. These are not Euclid's primitives,
but those that have arisen later as refinements from Euclid's work.

-   Point.

    -   Questions: What are points? Points of matter? Abstract objects?
        Points of space?

    -   Can we define point from more basic notions? Euclid defines a
        point as that which has no parts, taking the notion of parthood
        as more basic.

-   Congruence: a four place relation written $xy \sim zw$ meaning,
    intuitively, that the distance between $x$ and $y$ is the distance
    between $z$ and $w$.

    -   I have *explained* congruence in terms of distance, but that
        does not mean distance is more basic. We will congruence as the
        most basic notion in what follows, and we will later define
        distance in terms of it.

-   Betweenness: a three place relation, $\operatorname{Bet}xyz$ meaning
    $y$ is between $x$ and $z$.

    -   We can explain this in terms of $y$ lying on the straight line
        between $x$ and $z$, but again we should not take this to mean
        that the notion of a straight line is more basic. (We define
        straight line shortly in terms of betweenness)

    -   We understand betweenness to include the end points, so that $x$
        is between $x$ and $y$, and so is $y$.

## Discussion questions

-   Define region in terms of these basic notions. (A collection of
    points.)

-   Define straight line.

    -   (finite closed line: a region such that there exists $x$ and $y$
        and the collection consists of the points between them.

    -   Arbitrary line (open, closed, infinite): a region such that (i)
        for any three points on it, one is between the other two
        and (ii) for any two points in the region, *any* point between
        them is also in the region.)

    -   Infinite line (in both directions): for any two points on the
        line $x,y$, and arbitrary $z$ (not necessarily on the line) such
        that $y$ is between $x$ and $z$, $z$ is on the line.

-   The line $xy$ is at least as long as $zw$: (there exists a point $u$
    between $x$ and $y$ and $xu$ is congruent to $zw$.)

-   Sphere. (a region such that: there exists points $x$ and $y$ ($x$
    the center, $xy$ the radius) such that a point $z$ is in the region
    iff $xz$ is congruent to $xy$.

-   Plane: There exist distinct points $xyz$ such that a point is in the
    region iff it lies between two points that lie on any of the three
    infinite lines passing through $xy$, $yz$ or $xz$.

-   Circle: (definition of sphere with quantifiers restricted to a
    plane.)

-   Right angle. ($xyz$ is a right angle (at $y$) iff there exists a
    point $w$ such that $y$ is between $x$ and $w$, and $yx$ is
    congruent to $yw$ and $xz$ is congruent to $wz$.)

-   Parallel lines. (Euclid: Two lines in the same plane that never
    meet. Alt: lines in the same plane that can be connected by two
    right angles. Euclid's parallel postulate essentially says these two
    definitions coincide.)

-   Can you define betweenness from congruence? Yes. Note that $x,y$ and
    $z$ lie on the same line iff the sphere with a diameter $xy$ and the
    sphere with diameter $yz$ have one point in common. $y$ is between
    $x$ and $z$ if, additionally, neither $xy$ nor $yz$ are greater in
    length than $xz$.

## Euclid's postulates

Euclid's postulates. NB: Euclid's axioms are not complete, and not all
of his propositions strictly speaking follow from his axioms. It wasn't
until much later that logicians discovered how to axiomatize geometry
completely: see the Smith paper for an overview of the history. The
Tarski paper in dropbox gives an axiomatization in terms of congruence
and betweenness.

-   There exists a straight line between any two points.

-   Any stright line can be continued indefinitely.

-   For any point $x$ and $y$, there is a circle with center $x$ passing
    through $y$

-   Right angles are congruent (if $xyz$ and $x'y'z'$ are right angles
    and $yx\sim y'x'$ and $yz \sim y'z'$ then $xz \sim x'z'$.)

-   If two lines in a plane cannot be connected by a line that meets
    both at right angles, then they will eventually meet.

Application

-   Proof that there exists an equilateral triangle from the axioms.
    (Idea: given $xy$ consider the two circles with centers $x$and $y$
    and diamater $xy$. Either of the two points where they meet will
    form an equilateral triangle.)

-   Questions: how do we know those circles meet at all? Euclid's axioms
    do not seem to guarantee this.

# Non-Euclidean Geometries

There are many alternatives to Euclidean geometry. These can differ from
the theory we've presented above in a number of different ways:

-   One could have different primitives: instead of congruence and
    betweenness we might take notions like straight line and circle as
    basic (as Euclid did).

    -   Perhaps spatial geometry has *further* structure than congruence
        betweenness, and therefore needs further primitives. See
        'Kantian geometry' below.

    -   Or perhaps spatial geometry has *less* structure than Euclid
        thought. The view that it only has 'affine' structure---there's
        a notion of straight line, but no notion of equidistant
        points---could be captured by taking only betweenness as basic,
        and rejecting congruence. (Arguably the theory of space in
        general relativity can be thought of as like this: space itself
        only tells us which lines are continuous and smooth, as opposed
        to jagged, but does not supply us with notions like straightness
        or distance.)

-   One could have a different ontology:

    -   One might reject the existence of points: see the Tarskian
        'gunky' geometry below.

    -   One might reject regions that are infinitely extended: see
        Aristotelian geometry below.

    -   Or perhaps the only geometric shapes or solids there are are
        occupied by matter, so that the only way to talk about 'regions'
        is to talk about material objects. This is the Leibnizian
        picture.

-   Finally, one could accept the ontology and ideology of Euclid, but
    reject specific axioms.

    -   Example: the Poincare disc model described below.

## Aristotelian potentialism

1.  A region is bounded when there is a ball (defined using congruence
    and betweeness) such that every point in the region is in that ball.

2.  Aristotle did not believe there were infinite objects: every shape
    is finite or bounded, so there are no infinite lines, planes, or
    other regions.

3.  As far as I know Euclid believed this as well: the propositions of
    the Elements do not seem to require one to ever talk about infinite
    lines or regions.

    -   In fact, one of Euclid's common notions IV seem to imply that
        certain infinite shapes do not exist.

    -   The principle that if equals be added to unequals (common
        notion IV) the sums will be unequal.[^2] Take two rays (infinite
        line in one direction): they are equal because they can be
        superimposed, but adding unequals to them yields equals.

4.  There are variants of Euclidean geometry where the only regions that
    exist are bounded.

5.  NOTE: all the principles stated in terms of points, congruence and
    betweenness remain valid. It is principle concerning regions and
    containment of one region in another that change.

    -   Question: for any collection of regions, is there a region
        containing all of them? Find a counterexample.

    -   Question: how could we restate the parallel line postulate
        without positing infinite lines? (One way to state the postulate
        is to say that two infinite lines in a plane either meet or can
        be connected by a straight line intersecting both at right
        angles).

## Discrete space

## Tarskian gunky geometry

-   Rejects the existence of points.

-   Point cannot be a primitive so we need new primitives.

-   Primitives: being an open ball (i.e. the insides of a sphere, not
    including the boundary), the notion of a ball being contained in
    another.

-   We can reconstruct all of Euclidean geometry from this primitive.

    -   Two balls $a$ and $b$ are disjoint iff there is no ball
        contained in both.

    -   Two balls, $a$ and $b$, touch externally iff they are disjoint,
        and for any pair of balls containing $a$ but disjoint from $b$,
        one of the pair is contained in the other.

    -   Two balls, $a$ and $b$, touch internally iff $a$ is a part of
        $b$ and for any pair of balls containing $a$ and contained in
        $b$, one of the pair is contained in the other.

    -   Two balls $a$ and $b$ touch $c$ externally on opposite sides of
        $c$ iff they both touch $c$ externally and for any two balls one
        containing $a$ and disjoint from $c$, the other containing $b$
        and disjoint from $c$ will be disjoint. (They both touch $c$
        internally on opposite sides if the same holds, with
        'internally' replacing 'externally').

    -   Given two balls $a,b$, with $a$ contained in $b$, they have the
        same center (are 'concentric') iff any two balls both touching
        $a$ externally on opposite sides of $a$, and touching $b$
        internally, will touch $b$ internally on opposite sides of $b$.

    -   The centers of $a$ and $b$ are the same distance from the center
        of $c$ iff there is a ball concentric with $c$ and there is no
        ball concentric with $a$ or $b$ which is contained in or
        disjoint from that ball.

-   Using just the notion of a ball and containment we have defined
    equidistance. It is then possible to define congruence and
    betweenness.

## Kantian geometry

-   An extra primitive $Lxyzw$: meaning $w$ lies on the left side of the
    plane defined by $xyz$. (i.e. if you place a left hand, place with
    $x$ on the palm, $y$ on the knuckle and $z$ on a finger tip, the
    thumb will be in the same side of the plane as $w$ is.)

## Leibnizian geometry

This is the odd one out: Leibniz did not believe in space, just matter.
Nonetheless, there could be points of matter, and one can still ask
whether two points of matter are congruent to another, or if one point
of matter is between another two, so that geometry could is still

-   The only solids are material objects. There are still points and
    lines, but they are complete contained in matter, and extend only as
    far as the matter they are contained in extend.

-   Question: what principles involving betweenness are true in the
    Euclidean view of space that fail in the Leibnizian view?

## Pac-Man geometry and Moebius strips

-   The Pac-Man geometry: wraps around.

    -   One can represent it in three dimensional space as the surface
        of a donut.

        -   (Why not a sphere? No curvature.)

    -   The Moebius strip and Klein bottle: like the Pacman geometry
        except doing one trip to your starting position reverses left
        and right.

    -   Klein bottle is similar except it is a three-dimensional
        geometry.

## The Poincare disk model

(of two dimensional geometry):

-   Points are the points with in the unit disc

-   The straight lines are arcs of circles that are contained entirely
    in the disc and meet the boundary of the disc at right angles.

-   One $y$ is between $x$ and $z$ iff $y$ lies on the arc of the circle
    connecting $x$ to $z$.

-   $xy$ is congruent to $zw$ iff the arcs connecting $xy$ and $zw$ have
    the same 'hyperbolic length'.[^3]

# Numerical Representations of Space

## The Real Numbers and Pythagoras' Theorem

-   Whole numbers (\..., -2, -1, 0, 1, 2, 3, \...), the rationals
    ($\frac{1}{3}$, $\frac{3}{7}$, etc), the reals: $\mathbb{R}$.

    -   Numbers are abstract objects: they don't have locations, you
        can't see or touch them, they exist necessarily. Are they
        causally inert?

    -   We can depict them with a straight line, 0.

    -   Although points and regions of space share many things in common
        with mathematical objects, they are importantly different. You
        can visit points and regions of space, you cannot visit a
        number.

-   Properties:

    -   Question: What makes the real line different from a straight
        line in space? What further structure does the real line have?

    -   The reals come with two special operations, $+$ and $\times$,
        subject to certain laws. $a+b = b+a$, $(a+b)+c = a+(b+c)$, etc.

    -   There is a special real number, $0$.

    -   Question: what makes 0 special? (additive unit: $0+a = a+0$ for
        every real $a$. What makes 1 special? (multiplicative unit:
        $1\times a = a\times 1 = a$ for all $a$.

$\mathbb{R}^2$ and $\mathbb{R}^3$

-   $\mathbb{R}^2$ is the collection of all "ordered pairs" of real
    numbers. We notate the ordered pair of real numbers $a$ and $b$ with
    $(a,b)$ (note that $(a,b)$ is a different ordered pair than
    $(b,a)$).

-   $\mathbb{R}^3$ is similarly the collection of all ordered triples
    $(a,b,c)$.

-   We can represent them pictorially as *cartesian coordinates*

    -   Draw diagrams for: the $xy$ axis. The $xyz$ plane.

Pythagoras. (Note: although we are reasoning in terms of real numbers,
Pythagoras and the ancient geometers presented this all in terms of
geometrical shapes, like squares and triangles.)

-   First we begin with a theorem of Euclidean geometry: given a right
    angled triangle with sides of length $a,b$ and $c$ with $c$ opposite
    the right angle, the area under the square with side $c$ is the sum
    of the areas of the squares with sides $a$ and $b$ respectively.
    $c^2 = a^2 + b^2$.

-   Diagram: draw a square with sides divided: $b+a$ (left), $b+a$
    (top), $b+a$ (right) and $b+a$ (bottom). Draw four $abc$ triangles
    round the edge leaving a rotated square in the middle. Draw the same
    square with sides divided $b+a$, $b+a$, $a+b$, $a+b$ (with a $b$
    square in the bottom left and an $a$ square in the top right, and
    four $abc$ triangles in the remaining two rectangular spaces).

-   Pythagoras' theorem gives us a measure of distance between points.
    Let's start with $\mathbb{R}^2$.

    -   Question: what is the distance between two points
        $a,b\in \mathbb{R}$? $b-a$ where $b$ is the biggest of the two.

    -   Question: what is the distance between two points in
        $\mathbb{R}^2$ with the same $y$ coordinate, $(a,c)$ and
        $(b,c)$? Ans: $b-a$ (where $b$ is the biggest of the two).

    -   What about the distance between two points with the same $x$
        coordinate, $(a,c)$ and $(a,d)$? Same idea: $d-c$.

    -   The distance between $(a,b)$ and $(c,d)$. This line is the
        hypotenuse of a right angled triangle with the right angle at
        point $(c, b)$.

    -   What is the distance between $(a,b)$ and $(c,b)$? $c-a$.

    -   What is the distance between $(c, b)$ and $(c,d)$? $d-b$.

    -   By Pythagoras, the square of the distance between $(a,b)$ and
        $(c,d)$ is $(c-a)^2+(d-b)^2$. So the distance is the square root
        of this sum.

-   The same idea can be applied to $\mathbb{R}^3$: the distance between
    $(a,b,c)$ and $(a',b',c')$ is the square root of
    $(a'-a)^2 + (b'-b)^2 + (c'-c)^2$.

$\mathbb{R}^3$ is a model of Euclidean geometry

-   Question: what is a point? (A triple of numbers.)

-   What is congruence? ($xy \sim zw$ when the distance between $xy$ is
    the distance between $zw$: i.e.
    $(x_1-y_1)^2 + (x_2-y_2)^2 + (x_3-y_3)^2 = (z_1-w_1)^2 + (z_2-w_2)^2 + (z_3-w_3)^2$

-   Betweenness: $y$ lies on the straight line betweeen $x$ and $z$. We
    can give a numerical definition of this as well:
    $d(x,z)=d(x,y)+d(y,z)$.

-   IMPORTANT NOTE: Points of $\mathbb{R}^3$ are *not* the same of
    points of space!

    -   Triples of numbers are abstract objects and do not have
        locations. Points of space do have locations (in fact, they
        *are* locations).

    -   $\mathbb{R}^3$ has lots of extra structure that points of space
        does not.

    -   Question: what are they? Origin $(0,0,0)$? Why is 0 special in
        the real numbers (additive unit). Additive structure $+$?
        Distance?

## Representing points of Euclidean space with numbers

-   The directions up/down, left/right and forward/backward are special.
    You can get anywhere in space by following these three directions.

-   Given a starting point, and an orientation you can encode the
    position of any point of space with three numbers: a number of
    meters to go up (set it negative if you want to go down), a number
    of meters to go right (negative if you want to go left), and a
    number of meters to go foward (negative to go backwards).

-   Question: why do we need a starting point and orientation. (People
    in Australia have a different 'up', left and right depend on where
    you're facing)

Numerical representations of space

-   Let $E$ be the set of points of space.

-   A numerical representation of Euclidean space is a function $r$ that
    takes each point of space to a triple of real numbers
    (mathematicians would write this $r:E \to \mathbb{R}^3$).

-   For illustration we will map points of a plane to $\mathbb{R}^3$.

    -   Draw a diagram with with pairs of numbers labeling points of
        space (the board, a piece of paper).

    -   Question: what would be bad about representing the points
        $x,y,z,w$ (taken so that $xy$ and $zw$ are congruent on the
        board) with triples $(0,1)$, $(3, 10)$?

-   A function $r$ is a representation of space iff $r$ "preserves
    congruence and betweenness":

    -   For any points $x,y,z$ and $w$ of Euclidean space $xy\sim_E zw$
        iff $r(x)r(y) \sim_\mathbb{R} r(z)r(w)$.

    -   For any points $x,y,z$ of Euclidean space,
        $\operatorname{Bet}_E xyz$ iff
        $\operatorname{Bet}_\mathbb{R}r(x)r(y)r(z)$.

-   Given a numerical representation $r$, we can define a *numerical*
    notion of distance on points of Euclidean space

    -   The distance between points $x$ and $y$, relative to the
        representation $r$, is the distance between $r(x)$ and $r(y)$ as
        defined using Pythogoras (the square root of \...).

    -   Question: why is this notion of distance not unique?

Discussion questions:

-   There are *many* different numerical representations of space. How
    are they different?

-   Where does $(0,0,0)$ (the origin) get mapped to?

-   What is the orientation of the axes (which directions are we
    treating as up, left, and forward?)

-   Scale. Meters, yards, etc. These all determine different
    representation functions.

## Euclidean transformations and definability

An isometry is a map that takes points of Euclidean space to points of
Euclidean space and preserves shapes. It is a bit like a representation,
except we are mapping to points of space instead of numbers.
Nonetheless, we have to preserve congruence and betweenness:

A function $j:E \to E$ is a Euclidean transformation of space iff $j$
"preserves congruence and betweenness":

-   For any points $x,y,z$ and $w$ of Euclidean space $xy\sim_E zw$ iff
    $j(x)j(y) \sim_E j(z)j(w)$.

-   For any points $x,y,z$ of Euclidean space,
    $\operatorname{Bet}_E xyz$ iff $\operatorname{Bet}_Ej(x)j(y)j(z)$.

(Note that what I'm calling a Euclidean transformation is not quIte the
same as an isometry, which is the requirement that $Cxyj(x)j(y)$ for
every point preserving map. Isometries can't enlarge.)

Discussion question:

-   What are some examples of Euclidean transformations?

-   Shifts in various directions.

-   Rotations.

-   Reflections.

Discussion questions

-   Why must a circle get mapped to a circle?

Definability

-   A property is metaphysically definable from congruence and
    betweenness iff every isometry maps shapes with the property to
    shapes with the property.

-   Example: circle, straight line, (everything we've discussed in
    section 1).

-   Examples where the: being a line with the sahpe of the coastline of
    the west coast of the USA (a complex line, maybe even infinitely
    detailed). Can we define it with a finite sentence using only
    congruance and betweenness? Presumably not, but it is metaphysically
    definable since isometries preserve it.

    -   (More generally, a property is metaphysically defined from
        notions $X$,$Y$ and $Z$ iff every map that preserves $X$, $Y$
        and $Z$ maps shapes with the property to shapes with that
        property.)

    -   Question: described a mapping that only preserves betweenness?

Discussion question:

-   Why is circle metaphysically defined by congruence and betweenness
    according to our definition?

-   Can a circle be defined from betweenness alone? Find a betweenness
    preserving map that maps a circle to a non-circle. What about
    rhombus?

Example: Kantian geometry

-   Consider adding new primitive $Rxyzw$ to Euclidean geometry.
    Roughly, if you place your right hand on the triangle $xyz$ with $x$
    at the knuckle, $y$ at middle of the finger, and $z$ at the
    fingertip, $w$ will be in the same side of the place defined by
    $xyz$ as your thumb.

-   Is this definable from congruence and betweenness?

# Incongruent Counterparts

Reading: Van Cleve, 'Right, Left, and the Fourth Dimension'.

Kant argues against Leibniz for the thesis that Euclidean space exists.
In his argument he appeals to two shape properties: being the shape of a
left hand, and being the shape of a right hand. His argument, as
reconstructed by Van Cleve, proceeds as follows:

1.  There is a difference between the shape of a left hand and a right
    hand. This difference must either be due to the way the parts of the
    hand relate to one another internally, or due to how they relate to
    things that are not part of the hand---either other material objects
    or absolute space.

2.  The parts of a left hand are related to one another in the same way
    that the parts of a right hand are, so being left (or right) hand
    shaped cannot be a matter of the internal relations of the parts of
    the hands.

3.  A hand in otherwise empty space is either left or right, so it
    cannot be one or the other in virtue of its relation to other
    external material objects.

4.  Therefore a hand is left or right in virtue of its relation ship to
    absolute space.

## Different views, according to how they resist the argument

Note: the names 'Holism', 'externalism', etc. are Van Cleve's. It is not
important to learn these labels explicitly, just that you understand the
views and how they are different.

Holism:

-   rejecting premise 1. Perhaps being a left (right) hand isn't reduced
    to relations between the parts of the hand or other things, it is
    just basic unalyzed monadic property of hands.

-   VC: this contradicts mereological reductionism---the thesis that the
    properties of a composite whole are reducible to relations between
    its parts that do not have the property. But this isn't very
    decisive since mereological reductionism isn't very plausible.

    -   Question: Counterexamples?

    -   E.g. being red. All parts of a red thing are red. Having mass.

Internalism

-   Reject premise 2, there is an internal relation between

-   

Externalism

-   Reject premise 3.

-   What makes a hand left or right is its relationship too other
    material objects: clocks, doors, can openers, and so on.

-   A hand in empty space

    -   According to the externalist it is neither left nor right.

    -   But Kant thinks this is absurd: (i) in the imagination (when you
        picture it) the thumb either comes out of the left or the right
        hand side. (ii) if you were to introduce a body (by magic) into
        the space, it would either fit on to the heart side or the other
        side.

    -   Problem re (i): when you picture a hand you are inserting your
        self into the space in some way: you can picture it from above,
        behind, below etc. You could also insert yourself into the space
        in two mutually reflected orientations: one and the same hand
        would appear left or right depending on which way you insert
        yourself.

    -   Re (ii): CEM is a contentious principle of conditionla logic.
        Even if it is accepted, counterfactuals like this are usually
        thought to be indeterminate or chancy (would the coin have
        landed heads if it had been flipped, or tails?). Yet whether a
        hand is left or right is not an indeterminate or chancy matter.

Absolutism (accept the existence of space)

-   \...

-   But what then makes the difference between a left and a right hand
    shaped *region* (as opposed to the hand itself).

    -   If we appeal to the relation between the hand shaped region and
        absolute space, either that relation holds in virtue of the
        internal relation of the parts of that the region, or with
        external relations to space outside the hand shaped region. The
        same issues arise.

    -   (Perhaps there's a 'meta-space' in which regions of space are
        located? but then a regress ensues.)

-   It seems we need a space with more geometric structure than
    Euclidean space: the Kantian space described above (with an extra
    primitive $Rxyzw$ would suffice, for instance.)

    -   $Rxyzw$ means that none of $x,y$ and $z$ are between the other
        two, and the plane defined by them contains $w$ on the right
        hand side (inclusive). (On the side of the thumb if you place
        the palm at $x$, knuckle at $y$ and finger tip at $z$.)

    -   Axioms:

        -   If $Rxyzw$ then $x$ is not between $y$ and $z$, $y$ is not
            between \...

        -   If $Rxyzw$ then $Rzxyw$.

        -   $Rxyzw$ and $Rxyzw'$ if and only if, for any $u$ between $w$
            and $w'$, $u$ is not on the $xyz$ plane unless $w$ or $w'$
            are.

        -   $Rxyzz'$ or $Rxyz'z$.[^4]

        -   If $Rxyzw$ and $z'$ is on the $xyz$ plane, and the $zz'$
            line does not intersect the infinite $xy$ line, then
            $Rxyz'w$.[^5]

-   Problem: if $Rxyzw$ is a good notion for points in space, why
    couldn't the internalist say it makes sense for points of matter.
    Couldn't it be that there is a primitive internal relation like
    $Rxyzw$ that can be used to distinguish a left from a right hand.

## Handedness, The Fourth Dimension, Non-orientable spaces

The central idea: in certain spaces, one can transform a left hand on to
a right hand by a rigid motion (you can superimpose one on the other
just by movement in space).

-   Four dimensional space:

    -   The two dimensional analogue: reflecting an $L$ in a plane.

-   Non-orientable space

    -   Two dimensional analogue: adding a twist to the Pac-Man
        geometry.

    -   Note: the 2d moebius strip is usually represented as embedded in
        a 3d ambient space. Similarly, you can embed the 3d versions in
        a 4d space. However, (contrary to van Cleve), you do not need an
        ambient higher-dimensional space to have a non-orientable space.
        They were first discovered in this context, but their geometry
        can be described intrinsically without reference to the space it
        is embedded in..

Common objection

-   In four dimensional space you can take four straight sticks and
    arrange them so that each one is at right angles to all of the
    others.

-   Isn't this somehow inconsistent or incoherent?

-   No: we can use models to show that no contradiction follows from the
    Euclidean axioms and this idea

    -   Recall how we modeled 3D euclidean geometry using triples of
        number $(x,y,z)\in \mathbb{R}^3$. We were able to represent
        congruence and betweenness in this model by defining distance
        using Pythagoras' theorem.

    -   We can model 4D space using quadruples of number $\mathbb{R}^4$.
        Pythagoras' theorem gives us a notion of distance, and thus
        congruence and betweenness.

    -   Recall how 'rightangles to' can be defined from congruence and
        betweeness. It is possible to show that the points $(1,0,0,0)$,
        $(0,1,0,0)$, $(0,0,1,0)$ and $(0,0,0,1)$ are all at rightangles
        (using this notion of congruence and betweenness) when you draw
        the line from them each to $(0,0,0,0)$.

    -   All of the axioms of Euclidean geometry continue to hold (apart
        from one stating that space is 3D).

## Implications for various views

Why is this a problem? Who is it a problem for?

-   It is a problem for views that maintain that a hand in empty space
    is either left or right.

-   Q: which views maintain this? (Holism/internalism, Kant's version of
    absolutism.) Externalism is left in tact.

What each view predicts about 4d space/Moebis space is worth considering
separately.

A problem for internalists/holists

-   A rigid motion preserves all the internal geometric relations
    between a hand and itself. So they cannot change. Yet a left hand
    can be rigidly moved onto a right hand. So left and right cannot be
    a matter of internal geometric relations.

A problem for Absolutists like Kant

-   Is $Rxyzw$ well defined in four dimensions, or non-orientable
    spaces?

Externalism

-   Seems to be unscathed.

-   Qu: why?

    -   Rigid motions change the relation of a hand to external things.

    -   Explain how you could change a left hand into a right hand,
        using externalism to justify the claim that it is a left hand
        before, and a right hand afterwards.

    -   Are there universes where we couldn't justify this? (It works
        well iff all the clocks, door, can openers, etc, all lie iin the
        same 3d plane. Not so good if not.)

-   What about externalism in Moebius space? If material objects like
    hands, torso's, clocks and so on, are located uniformly throughout
    space, it's hard to say whether a hand is left or right by its
    relations to other material things (perhaps they are neithr). If
    they are all close to one another, one might define a hand as left
    or right by its relations

    -   Toy model of externalism: two objects have the same handedness
        iff there is a small region (say, a ball with diameter less than
        half the length of a trip around the universe) such that they
        can be superimposed using rigid motions *that stay inside that
        region*. If all the material are close, this is an equivalence
        relation.

## Nerlich's argument

We identified two problems with Kant's argument

1.  In order for a hand to be left or right in virtue to its relation to
    space, there must be more structure to space than the Euclidean
    structure (congruence and betweenness). Above we appealed to the new
    primitive $R$. But if that's OK, why can't the internalist do the
    same thing? Help themselves to a four place primitive $Rxyzw$
    between points of *matter*, instead of spatial points?

2.  The proposed extra primitive $Rxyzw$ isn't even coherent in 4
    dimensional spaces, or in Moebius universes so Kant's position that
    a hand in empty space is *always* either left or right is not
    sustainable.

Nerlich's argument is an argument for absolute space that avoids these
problems with Kant's argument. Instead of working with the left right
distinction, he works with a distinction that makes sense even in four
dimensional and Moebius universes. First, some definitions

1.  Recall that an incongruent counterpart of an object is another
    object that (i) has the same shape (i.e. shares all properties
    metaphysically definable from things like congruence and
    betweenness), but (ii) cannot be superimposed on the original using
    only rigid motions.

2.  An enantomorph is an object that could have had an incongruent
    counterpart.

3.  A homomorph is an object that couldn't have had an incongruent
    counterpart.

Examples, exercises

-   Is a ball in empty Euclidean space a homomorph, or an enantomorph?

-   What about a hand in empty Euclidean space?

-   What about a hand in Moebius space?

-   What about a hand in four dimensional space?

-   Are there any enantomorphs in four dimensional space? (Answer: yes.
    An analogue of a four dimensional hand.)

-   Are there are enantomorphs in Moebius space? (Answer: Yes! While all
    bounded objects are 3d, and can be "reflected" by one trip around
    space, you can two rings that go around the whole space with
    opposite facing arrows heads (triangles) attached to each.)

Here is Nerlich's variant argument.

-   A hand in empty space is either a homomorph or an enantomorph.

-   This cannot be explained by the internal relations of the hand to
    itself.

-   Nor to external material objects (there are none).

-   So it must be because of its relation to an absolute space: the
    distinction between 4D and 3D is one of the ambient space, similarly
    the distinction between Orientable and non-orientable.

Essentially, whether an object is an enantomorph on not is not intrinsic
to the object itself --- it depends on the global structure of space. If
it is 4D or Moebius space a hand is a homomorph, whereas the exact same
shape is an entantomorph is ordinary Euclidean space.

# Newton's first law, substantivalism and relationism

In these lectures we will state and discuss Newton's first law of
motion. We will then state two theories of space and time, one due to
Newton, the other to Leibniz, and we will see how to formulate Newton's
law in both of these theories.

## Pre-Newtonian Physics

Newtonian physics is a theory about the motions of objects. A natural
question to start with:

-   What are the 'natural' motions of things? I.e. how do things move
    when they are not being acted on by other forces -- being pushed,
    etc.

Aristotle:

-   There are different elements such as earth, fire, wind, water and
    aether.

-   The universe has center (namely the center of the earth).

-   The natural motion of earth and water is to move towards the center
    (i.e. down).

    -   Earths inclination towards moving down trumps waters
        inclination. Thus a stone will sink in water.

-   The natural motion of fire and air is away from the center (i.e. up)

    -   Fire's inclination towards moving up trumps airs inclination.
        Fire rises above air.

-   Finally there is aether--the substance from which the sun, moon and
    stars are composed--whose natural motion is circular about the
    center of the universe

Question:

-   Does congruence and betweenness exhaust all the relevant properties
    of Aristotelian space?

-   (No, there is a special point, the center to the universe, that is
    needed to explain the natural motions of objects).

Gallileo's view was that the natural motion of all objects was circular,
about the center of the earth.

-   See the experiments on inclined bodies in Maudlin p18.

## Newton's first law

Newton's first law (Maudlin, p.4).

-   Every body perserveres in its state either of rest or of uniform
    motion in a straight line, except insofar as it is compelled to
    change its state by impressed forces.

Thus, the natural motion of a body (absent other forces) is in a
straight line.

Observation

-   This principle governs *all* matter alike. This ideas wasn't that
    mainstream until Newton. The Aristotelian world view has different
    laws for different sorts of objects.

Counterexamples, implications and clarifications?

-   We know what straight line means. What does uniform motion mean?
    Informally (for now) constant velocity.

-   Counterexample? According to the first law, if I throw an apple at a
    tangent to the earth it will follow a straight line into space and
    continue that way forever?

-   Counterexamples? If I let go of this apple, it will remain at rest?

-   Gravity is a force that acts on these objects.

-   If a throw an object in empty space, sufficiently far from earth,
    won't it eventually slow down? No. It does that on earth because of
    friction and air resistance, in empty space it will continue moving
    on a straight line forever.

    -   Newton's idea was quite radical: most of the objects we spend
        our time with are subject to gravity, air resistance and
        friction.

## Newton's metaphysics of space and time: Substantivalism

-   Substantivalism: the belief in the existence of points or regions of
    space, point or intervals of time.

According to Newton space is a three dimensional Euclidean space. Time
is a one dimensional Euclidean space. Objects (lets say, particles) are
located in space at different times.

-   Primitives

    -   Congruence and betweenness for points of space.

    -   Congruence and betweenness for times.

    -   The property of being a particle.

    -   A ternary relation $L$ telling us which point of space each
        particle is located at at each time: $Lapt$ means the particle
        $a$ is located at the point $p$ at time $t$.

Let's analyze the first law

-   Define what it means for a particle to be at rest using the
    primitives.

-   Define what it means for a particle to be moving at a constant
    velocity. ((i) If $tu$ and $sv$ are congruent intervals of time,
    then the location of $p$ at $t$ and $u$ and at $s$ and $v$ are
    congruent. (ii) the locations of $p$ all lie on a straight line.
    Note that without (ii), one could have $p$ moving at a constant
    speed in a circle, and without (i), you could have $p$ accelerate on
    a straight line.)

-   Harder: say what it means for one particle to be moving twice as
    fast as another.

A question to think about (which we'll return to): is the notion of
being at rest in good standing? (If it is, absolute rest is certainly
not the every day notion, because the earth is rotating around the sun.)

## Leibniz's theory of space and time: Relationism

According to Leibniz there are no points or regions of space or time.
There are just relations between material objects (say, particles). This
view is called Relationism.

What sort of relations could these be, and how could we state Newton's
laws in terms of them. There are several options concerning what we
might take to be laws.

-   Posit mathematical objects, like real numbers.

-   Distance, relating two particles to a real number, the distance
    between them.

-   How to make sense of temporal relations? Maybe we should be thinking
    on terms of pointlike events, that exist only at a time, rather than
    pointlike particles that persist through time? A particle consists
    of a continuum of such events.

    -   In the philosophy of time, this view about material objects is
        called the perdurantist theory of persistence.

Discussion questions

-   Is it possible to define being at rest? from these primitives.

-   Can a particle in otherwise empty space be at rest or not?

-   What about relative motion? One particle is moving relative to
    another at 5m

# The shift argument

Leibniz notes that if Newton's theory of space and time were correct
then there are a great many situations that are indistinguishable.

1.  Shifts and rotations. God could have created the entire universe
    five meters away (in some particular direction) from where it is in
    fact created, but kept the arrangement of material objects the same.
    Or he could have rotated the universe.

2.  Reflections. God could have created the universe with the material
    objects arranged in the present way, but reflected about some plane.

3.  Time shifts. He could have created the universe a year earlier than
    he in fact did, but kept the history of events and things the same.

4.  Velocity boosts. He could have created the universe as it in fact
    is, but added a constant velocity in some particular direction to
    every object.

5.  Time reversals?? A temporal reflection. You could imagine the entire
    history of the universe reversed, so that all events appear in the
    opposite order.

    -   NB: Leibniz does not make this argument, and Newton appears to
        hold that time has a favoured direction so that that time is not
        homogenous. But note that $E^1$, one dimensional Euclidean
        space, doesn't have a preferred direction, so Newton's actual
        laws don't actually favour one direction.

    -   Note that time reversal doesn't apply to the gravitational
        equations: massive objects will repel each other rather than
        attract. The time reversal invariance of Newtonian mechanics
        means: if one system of motions is possible (for some force
        field on space), then there is a force field relative to which
        the reversal is.

Things to note about these possibilities

-   All of the operations described above are what are called
    *symmetries* of Newton's laws. This means, if a system obeys those
    laws ($F=ma$, and so on) then uniformly shifting or rotating the
    system will yield a system that also obeys those laws.

    -   Example: two bodies orbiting one another.

    -   Non-example: stretch along one dimension -- the result won't be
        law like.

-   The worlds related by these symmetries are observationally
    equivalent. (remember, you the observer, are one of the things that
    is shifted, reflected, boosted, etc.)

-   The arguments rest on the assumption that space (and time) is
    homogoneous and isotropic, and reflection invariant.

    -   Leibniz: 'One point in space does not absolutely differ in any
        respect whatsoever from another point of space'. A space is
        homogenous iff a translation is a Euclidean map (preserves the
        geometrical primitives, such as congruence and betweenness, and
        any other). It is isotropic iff translations preserve the
        primitives. And reflection invariant iff reflections preserve
        the primitives.

    -   Euclidean space is all three.

    -   What about Aristotelian space? It is not homogenous but it is
        isotropic.

    -   What about Kantian space?

-   In general relativity space is not in general homogenous or
    isotropic.

Question:

-   How do these examples rest on absolute space? Does the relationist
    accept these variants of the actual universe? If not, why not?

There are several different arguments against absolute space and time
that use these possibilities in subtly different ways, and are thus
quite easy to conflate. For concreteness we will focus on spatial
shifts.

## The Principle of Sufficient Reason

Archimedes:

-   Consider a scale with two identical weights on either side. The
    system must be in equilibrium (i.e. it won't tip one way or the
    other), for there is no reason that it tip one way over the other.

The principle of sufficient reason

:   There must be a sufficient reason why things are so, rather than
    otherwise.

It is a strong principle of cause and effect.

Could we avoid the PSR argument by denying the existence of God?

-   Perhaps there was no moment of creation. The positions of things now
    are explained by their earlier positions. And there was no first
    time so there is no .

-   But then the position of the system as a whole at all times could
    still be shifted.

Implications of the PSR

-   No indeterminism.

    -   But in quantum mechanics one can have chancy coin-flip like
        events, where two outcomes are equally likely, and no reason
        exists for one over the other.

    -   Another theory: parallel universes (so no real indeterminacy. No
        asymmetry because both outcomes happen.

-   If the PSR is true there must be a reason the universe is exactly
    how it is and not otherwise. Leibniz suggests this is because the
    universe is the best of all possible worlds -- if things were
    different somehow then the universe would be worse off, so there is
    a reason God made things this way.

    -   Is it plausible that we're living in the best possible world?
        What about wars, poverty, inequality, etc?

-   If the PSR is true its truth is very fragile. A slight change ---
    e.g. if I sneezed a moment earlier, or I set my cup down a
    millimeter from where I actually put it --- the universe would be
    different and have been optimal, violatig the principle of
    sufficient reason.

    -   Given that there's a very high chance that the universe will go
        differently from how it in fact will go, and the PSR is false in
        any possibility where the universe has gone differently, the
        chance of the PSR is incredibly low.

## The Identity of Indiscernables

The principle of identity of indiscernables

:   No two things can be completely qualitatively alike.

What is a qualitative property?

-   A property that doesn't involve reference to other individuals.

    -   Examples. Being taller than Mary (not qualitative), being taller
        than someone (qualitive).

    -   Linguistic test: does the property involve proper names? What
        about being German? (Seems to involve reference to Germany.)

-   The principle is trivial without the restriction to qualitative
    properties

    -   If $a$ and $b$ share all properties, then they must share the
        property of being identical to $a$, which $a$ has. Then it
        follows that $b$ has it too.

The Newtonian view violates the principle of identity of indiscernables

-   A world like ours, and a shifted world are qualitatively
    indiscernable, yet they are different due to the positions of
    particles.

-   But is the PII a good principle?

    -   Max Black's spheres. Aren't they qualitatively indiscernable?
        But surely they're possible.

-   Note that empty Euclidean space also violates the PII: every point
    of space is indiscernable from any other point.

## Unobservables, Occams razor

The absolute theory of space and time posits unobservables.

-   Examples of unobservables:

    -   The location of a particle: can we know which particular
        spacetime point a particle is located based merely on
        observations?

    -   The absolute velocity of a particle.

-   Examples of observables:

    -   The distance between two particles.

    -   The relative velocity of one particle relative to another.

Verificationism: there are no unobservable facts.

-   Verificationism widely rejected: best physical theories often need
    to posit unobservables to give simple accounts of the observable
    phenomena.

-   The relation between the observables and unobservables is clear: the
    observable distance between two particles is determined by their
    locations (unobservable), and the distance between those. The
    observable relative velocity of two particles is the difference
    between their absolute velocities.

Nonetheless, we shouldn't posit unobservable facts that don't do any
work.

-   Example: imagine adopting Newton's worldview but positing a special
    spatial point, the origin, relative to which every thing has an
    'absolute distance'. This postulate doesn't do any work, and
    complicates the theory unecessarily.

-   Occams razor: look for explanations that use the smallest possible
    set of elements

    -   In this case, use the minimum set of primitives needed.

Remaining questions:

1.  If the relationist could account for Newtonian physics without
    positing absolute space, then by Occam's razor it should be
    preferred. But can one carry out Newtonian physics in the
    relationist framework? This is the topic we'll turn to next.

2.  It seems (and we will justify this later) that position in space is
    necessary to do physics in the simplest way. But there are some
    aspects of Newton's picture that can be eliminated without affecting
    his physical story. An importantt example is absolute rest---we will
    see how an alternative to Newton's metaphysics of space and time,
    using a single spacetime, lets us achieve the same physical
    predictions with fewer unobservable notions like absolute rest.

# Newton's Bucket

## Newton's second law

Aristotle's theory of motion

-   We might summarize it with the equation $F=mv$. Was pretty much
    going theory up until Newton (Bradwardine proposed a logarithmic
    theory of the relation between force and velocity.)

-   According to this theory, if you apply a constant force to an object
    it will move at a constant velocity. When you stop applying force it
    will come to a halt (not immediately: later Aristotelians, such as
    John Philoponus and Ibn Sina, thought that the application of force
    imparted something called 'impetus' to the object for a little
    while).[^6]

-   Problems explaining the motions of the planets uniformly? (Aristotle
    had an explanation: they were made of aether, whose natural motion
    was circular, but this explanation was not uniform -- it applied to
    some objects but not others).

Newton's second law

-   $F=ma$. If you apply a constant force to a body it will change
    velocity at a uniform rate in the direction of the force, and in
    proportion to the amount of force and the mass of the object.

-   The observations in favour of Aristotle's theory can be accounted
    for by friction.

-   Questions: Consider a particle moving at a constant velocity
    travelling east

    -   Apply force in an eastward direction. What will happen?

    -   Apply force in a westward direction. What will happen?

    -   Apply force in an southern direction. What will happen?

    -   Apply force in a southeast direction. What will happen?
        (components)

Circular motion

-   Suppose you have a particle travelling eastward at a constant
    velocity. What forces would you have to apply to it to ensure that
    it travels in a circular motion at a constant speed?

    -   At $t_0$ it cannot be, e.g. southeast, because that would have
        an eastward component, and increase the speed. cannot be
        southwest either, so it must be at right angles -- i.e. south.

    -   After the particle has changed direction somewhat, the force
        cannot still be acting south, otherwise it will impart a
        component that will speed the particle up (as above). By the
        same reasoning it must still be at right angles

    -   Thus the force must always be at right angles to the velocity,
        and so must be changing direction with the path the particle.

-   Newton's yoked globes

    -   Two globes (of equal mass) attached by a cord, with an initial
        velocity perpendicular to the cord.

    -   The cord will exert a force at right angles to the globes at all
        times, and so they will travel in circular motion.

-   Clarke discusses a similar phenomenon in his correspondence with
    Leibniz: if a bucket filled with water rotates, the water will move
    towards the edges..

## A problem for relationism?

The problem for the relationist

-   Consider a world with two yoked globes in otherwise completely empty
    space rotating, and then consider a world where they are not
    rotating.

-   According to Newton there should be tension in the cord in one world
    but not the other.

-   But there is (apparently) no relationist difference between the two
    worlds.

Possible responses

-   Option 1: Deny that there is a difference between these two
    universes.

    -   Leibniz takes this option: he simply repeats the argument from
        the PSR and PII.

    -   Note that there are two options: either yoked globes in
        otherwise empty space have tension in the cord, or yoked globes
        in empty space do not. Which should we go for?

    -   Problem: when we actually perform the experiment, there is a
        difference between rotating and stationary yoked globes. How
        should we explain this?

        -   Mach: by the relation to the background stars.

        -   According to Mach there is no difference between spinning
            the globes vs keeping the globes stationary and spinning the
            stars around it. Both would cause tension in the cord.

        -   Important note: Newton's theory and Mach's theory offer
            different physical predictions, for instance, about globes
            in empty space (Newton says that you can have rotating
            globes, and there would be tension whereas Mach denies
            this).

        -   The problem is Mach didn't have a worked out relationist
            theory to replace Newton's.

-   Option 2: accept that there can be differences between the rotating
    and stationary yoked globes, but posit more structure (i.e. more
    primitives) that explain the difference

    -   Note that the new primitives should be acceptable to the
        relationist --- they mustn't rely on absolute space, or things
        like that.

    -   Possibility 1: there are primitive and explained forces in
        addition to distance relations between material bodies. The
        difference between the two worlds is then just a matter of there
        being tension in the cord in one world, and not in the other.

        -   Somewhat unsatisfactory. Newton is able to *explain* why
            there are forces in one case, but not the other, in terms of
            the motions of the globes. Here we have no such
            explanations.

    -   Possibility 2: the relationist could adopt a perdurantist theory
        of material objects, in which they are composed out of temporal
        parts. In the first world the globes have a helix structure,
        where as in the second they draw out parallel straight lines in
        time.

        -   By positing suitable kinds of geometry primitives can
            distinguish between helixes and parallel straight lines.
            (Note that the naive way of doing this commits the
            relationist to a notion of absolute rest -- but there should
            be a way around this.)

# Galilean spacetime

Galileo's experiment

> For a final indication of the nullity of the experiments brought
> forth, this seems to me the place to show you a way to test them all
> very easily. Shut yourself up with some friend in the main cabin below
> decks on some large ship, and have with you there some flies,
> butterflies, and other small flying animals. Have a large bowl of
> water with some fish in it; hang up a bottle that empties drop by drop
> into a wide vessel beneath it. With the ship standing still, ob serve
> carefully how the little animals fly with equal speed to all sides of
> the cabin. The fish swim indifferently in all directions; the drops
> fall into the vessel beneath; and in throwing something to your
> friend, you need throw it no more strongly in one direction than
> another, the dis tances being equal; jumping with your feet together,
> you pass equal spaces in every direction. When you have ob served all
> these things carefully (though there is no doubt that when the ship is
> standing still everything must happen this way), have the ship proceed
> with any speed you like, so long as the motion is uniform and not
> fluctuating this way and that. You will discover not the least change
> in all the effects named, nor could you tell from any of them whether
> the ship was moving or standing still. In jumping you will pass on the
> floor the same spaces as before, nor will you make larger jumps toward
> the stern than toward the prow even though the ship is moving quite
> rapidly, despite the fact that during the time you are in the air the
> floor under you will be going in a direction opposite to your jump. In
> throwing something to your companion, you will need no more force to
> get it to him whether he is in the direction of the bow or the stern,
> with yourself situated opposite. The droplets will fall as before into
> the vessel beneath without dropping toward the stern, although while
> the drops are in the air the ship runs many spans. The fish in their
> water will swim toward the front of their bowl with no more ef fort
> than toward the back, and will go with equal ease to bait placed
> anywhere around the edges of the bowl. Finally the butterflies will
> continue their flights indifferently to ward every side, nor will it
> ever happen that they are con centrated toward the stern, as if tired
> out from keeping up with the course of the ship, from which they will
> have been separated during long intervals by keeping themselves in the
> air.

Example: three worlds containing two spaceships $A$ and $B$ approaching
one another.

1.  $A$ is stationary $B$ is moving west at 10m/s

2.  $B$ is stationary, $A$ is moving east at 10m/s

3.  $A$ is moving east at 10m/s, $B$ is moving west at 10m/s.

These cases are observably indistinguishable. Why?

-   According to Newton there is a difference between these three
    scenarios

    -   Question: Using Newton's primitives , state something that's
        true in scenario 1 that is false in scenario 2. (Newtonian
        primitives: particle $p$ is located at point $x$ at time $t$,
        spatial congruence and betweenness, temporal congruence and
        betweeness).

    -   Note that this means that you can't avoid absolute rest in
        Newtonian physics.

## Galilean spacetime

-   Newtonian space + time

    -   Diagram: 1D time + 3D space (both Euclidean)

    -   Material objects move about in a single 3 dimensional space. At
        two times you can ask whether a particle is located at the same
        point of space, or different points of space.

-   Galilean spacetime

    -   No 1D manifold for time. Infinitely many 3D Euclidean spaces,
        one for each time in Newton's theory. We will call these
        'slices'.

    -   A particle has a position in exactly one of these spaces.

-   Qu: why does the Newtonian definition of absolute rest fail.

-   Spacetime events:

## Similarities and differences between spatial points and spacetime events, times and timeslices

We call the points of a given timeslice "spacetime events". This is a
technical word -- they are not events in the ordinary sense

-   We think of the points of these slices as ideal 'events': they not
    only have a location, but a time.

-   They are ideal in the sense that they occur instantaneously, and
    have no extension. They also 'occur' even if there is no physical
    event happening there.

-   Consider me snapping my finger: there is an instantaneous space time
    event that coincides with it, and occurs even if I hadn't snapped my
    finger. In this slightly strange sense, then, there are spacetime
    events occurring even in empty parts of space.

-   don't attach too much significance to the name, just think of it is
    a suggestive word for these things (they are like events in the
    sense that they have a place and a time that they occur).

Spatial points vs spacetime events

-   -   Similarity: At a given time, both act as "places", locations for
        material objects to occupy. They are both spatially
        dimensionless (they are not spatially extended).

    -   Difference: spacetime events exist exactly in history --- they
        flash in an out of existence instantaneously. Spatial points
        always exist.

-   -   Similarity: At any given time (i.e. in any time slice) there is
        a notion of spatial distance between spacetime events occuring
        simultaneously. Just as there is between points of Euclidean
        space.

    -   Difference: Since spatial points always exist, we can compare
        the distance between points relative to different times. By
        contrast, we cannot talk about the distance between
        non-simultaneous spacetime events. (why not?)

-   -   Similarity: Objects have locations at both spatial points and
        spacetime events.

    -   Difference: An object can only be located at a spacetime event
        at most once in its lifetime (because spacetime events exist
        only once).

Times vs timeslices.

-   -   Similarity: They both act as answers to 'when' questions. They
        keep track of the order of physical events.

    -   Difference: Times are pointlike (they are point of a 1D
        euclidean space). Timeslices are infinite 3D manifolds with lots
        of pointlike events as parts.

-   -   Similarity: There is a notion of temporal congruence and
        betweenness between times and points of space.

## Primitives for Galilean spacetime

What primitives should we posit? Some deciderata:

-   We need to say what it means for a particle to be moving in uniform
    motion (it appears in Newton's first law)

    -   Qu: why can't we say that its trajectory is a 'straight line',
        and employ the usual Euclidean definition of straight line in
        terms of spatial betweenness?

    -   Ans: because a particle doesn't draw a straight line in any of
        the 3D slices. It has at most one location in each slice.

-   We don't want to introduce primitives that let us reinstate the
    notion of absolute rest.

    -   Qu: What primitives might do this?

    -   Example: one way would be if I could talk about "absolute
        distances" between points belonging to different slices. If the
        distance between the locations of a particle in any two slices
        is 0 , then we know that it is at absolute rest.

    -   An absolute notion of congruence for spacetime points, letting
        you talk about congruence between four points in four
        potentially different slices, would allow this (Qu: why? ans:
        $xy$ is congruent to $zz$ means the distance between $x$ and $y$
        is 0.)

-   We also want each slice to have a Euclidean geometry, so that we
    have a notion of congruence between four points *in the same slice*.

    -   One could do this by brute force, but it will turn out there's a
        more general primitive that will let us recover the Euclidean
        primitives for each slice.

So what are the required primitives?

1.  Similar to Newton, we need a primitive, $L$, telling us where each
    particle is located in each slice.

2.  $UBet\, xyz$ intuitively means $x$, $y$ and $z$ lie on a trajectory
    of uniform motion (from different slices), and $y$ is between $x$
    and $z$.

    -   Note how the informal explanation assumes the notion we are
        trying to define. The order of explanation doesn't have to
        reflect what is more fundamental than what.

    -   Qu: how does this help with the first issue of defining a
        particle moving in a straight line from location and UBet?

3.  Given four points $xyzw$, potentially different slices, we have a
    notion of temporal congruence, $xy\sim_t zw$, meaning the time
    elapsing between the events $x$ and $y$ equals the time elapsed
    between events $z$ and $w$.

4.  Given four points $xyzw$ where $x$ and $y$ are in the *same* slice,
    and $z$ and $w$ are in the *same* slice, we have a notion of spatial
    congruence $xy\sim_s zw$

    -   Intuitively $xy\sim_s zw$ means $x$ and $y$ are in the same
        slice, and $z$ and $w$ are in the same slice, and if you had a
        rigid rod that extended between $xy$ you could wait some amount
        of time (until $z$ and $w$ occur) and using rigid motions place
        the rod so that it extends between $z$ and $w$

    -   Note that this way of explaining things just doesn't make sense
        if $x$ and $y$, or $z$ and $w$, belong to different slices. (A
        rod is only ever located in one slice at any given time).

Question:

-   Qu: Why is Galilean spacetime different from $E^4$ (four dimensional
    Euclidean space), plus a 'foliation' of $E^4$ it into lots of
    parallel 3D Euclidean slices?

-   Ans: you have congruence for arbitrary elements of $E^4$, so you can
    say that $x$ and one slice, and $y$ in another slice are 'at the
    same place': $xy \sim_s xx$.

## Representations of Galilean spacetime and transformations

Note that in a given *spacetime diagram* of Galilean spacetime, it seems
as though we do have a notion of absolute rest. But actually that is an
illusion: there are lots of equally good ways to represent Galilean
spacetime by a drawing. Some might place the point $x$ above $y$, other
might not.

We can make this precise by talking about representation functions
mapping points of space to quadruples of real numbers $(x,y,z,t)$.

-   TODO

# Nominalism and quantities

The abstract concrete distinction. Concrete objects are the sorts of
objects you can bump into, see or hear, that it makes sense to ask how
much they weigh, .

-   Abstract objects: properties (wisdom, the property of being red,
    etc), numbers and other mathematical objects

-   Concrete objects: tables, chairs, people, spatial points and
    spacetime events?

Here are two views:

Nominalism

:   Everything is concrete

Platonism

:   There are non-concrete objects.

Platonism attracts many questions -- for instance, if there are abstract
objects like numbers how do we get to know things about them? Let's
explore nominalism.

How to be a nominalist? Are there nominalistically acceptable surrogates
for mathematical claims. Goldbach's conjecture (every even number apart
from 2 is the sum of two primes), for instance, could still be
meaningful. Suppose there *could* have been any finite number of
oranges. There's an even number of oranges = you can evenly divide the
oranges into two bags (evenly divide means: you can pair the oranges in
one bag with the oranges in the other, by laying them out side by side).
There's a prime number of oranges: apart from put each orange in its own
bag, you can't evenly divide the oranges between any number of bags.

The indispensability argument:

1.  Our best physical theories entail the existence of numbers (and
    other abstract objects, like vectors etc)

2.  We have good reason to believe these theories.

3.  So we have good reason to believe in numbers.

To properly assess this argument we need

Two kinds of nominalism

-   Do we simply deny the existential statements of pure mathematics, or
    do we try to recover them?

-   Many nominalists try to find something nominalistically acceptable
    to replace mathematical claims (see, e.g., the attempts regarding
    Goldbach's conjecture above).

-   Field thinks we can simply deny them. What needs to be recovered,
    rather, are the .

## Quantities

Examples

-   Scalar quantities: Distance, mass, charge, energy,

-   Vector quantities: velocity, force.

-   Fields: the gravitational potential (scalar field), the
    gravitational field (vector field),

Background mathematics: introduction to vectors.

## Platonistic Newtonian physics

Warmup: the platonistic theory of geometry versus the Euclidean theory.

-   Primitives need: $Dxyz$ meaning the distance between the points $x$
    and $y$ is $z$

-   Ontology: real numbers in addition to space.

-   Draw picture of absolute space (or a timeslice) with numbers, with
    fundamental relations relating the two.

-   Q: in what way is the Euclidean picture different from from the
    platonistic version of geometry?

A collection of platonistic primitives needed to do Newtonian physics.

-   $Mxy$: the mass of the particle $x$ is the number $y$. (Often it is
    written as a function: $m(x)=y$)

-   $Dxyz$: the distance between $x$ and $y$ is the real number $z$.

-   $GPot\, xy$ the gravitational potential at the spacetime event $x$
    is the number $y$.

-   $GravField\,xv$ the gravitational field at the spacetime event $x$
    is the vector $v$

The theory.

-   The gravitational field (a vector field). This is determined by the
    $GravField$ primitive.

    -   The vector associated with any point is the gravitational force
        that would be exerted on a particle if it existed there.

-   The gravitational potential scalar field.

    -   The intuitive explanation of gravitational potential: first fix
        a starting point, $x$. The gravitational potential at $y$ is the
        amount of work done to move an object with unit mass from $x$ to
        $y$.

    -   We can also get a handle on it by its relationship to the
        gravitational field.

-   The relationship between them: a scalar field is like a terrain over
    space. The slope of that terrain at any given point gives us a
    vector so a suitable scalar field determines a vector field.

-   The gravitational field (or the gravitational potential) determines
    .

two things to note

1.  This sort of theory requires, in addition to particles and possible
    spacetime events, for tthere to be numbers, vectors, and so on.

    -   Thus we have to be platonists to accept this sort of theory.

2.  The fundamental primitives do not only hold only between physical
    objects (particles, spacetime events), they also relate the physical
    objects to numbers.

    -   Isn't it somewhat puzzling that numbers are appearing in the
        fundamental relations that explain, for instance, how physical
        things move?

    -   Surely if all numbers disappeared, the physical world could
        still behave as it in fact behaves? Planes wouldn't start
        fallinng out of the sky, the planets wouldn't start following
        non-elliptic curves, etc, if there hadn't been any numbers.

### The problem of scale for platonistic theories

-   Distance: if this is a fundamental ternary relation to numbers, it
    must relate any two particles to a unique number. But which number
    should it be? The distance between them in meters? or in yards? or
    in none of these. Why should it be one and not the other.

-   We earlier talk about mathematical representations

    -   A distance function $d$ mapping pairs of points to a number with
        the property that (i) $d(x,x)=0$, and (ii) $d(x,y)=d(z,w)$
        whenever $xy$ is congruent to $zw$.

    -   But there are lots of functions that satisfy these criteria, and
        we suggested they're all on a par.

    -   According to the platonistic theory, however, they're not all on
        a par. One of these functions is the actual *distance* between
        $x$ and $y$.

Gauge symmetry in the gravitational potential

-   Lowering or raising a terrain doesn't change the slopes.

Questions

-   Qu: Can you come different primitives relating material objects to
    real numbers that aren't subject to the problem of scale (for say
    distance).

-   Does this suggest that the gravitational field is a better
    fundamental entity that the gravitational potential?

Note that the Euclidean theory of space, in terms of congruence and
betweenness, doesn't have the problem of scale for distances.

### Nominalistic Approach to scalar fields

**A Tarski style approach to scalar fields.** Let's begin with a scalar
field like temperature. The platonist can respresent this by mapping
points of space or spacetime to real numbers, e.g. the temperature in
farenheit at that point (but notice that we have a problem of scale:
surely fundamental reality doesn't single out farenheit, over say
centigrade, as special here).

Hartry Field represents scalar fields with two primitive relations
between points of spacetime

-   $\operatorname{TCong}\, xyzw$ meaning the difference between the
    temperature at points $x$ and $y$ is the same as the difference
    between the temperature at $z$ and $w$.

-   $\operatorname{TBet} xyz$ the temperature at the point $y$ is
    between the temperature at $x$ and at $z$.

One question Field remains open on is whether there is a well-defined
notion of 'greater temperature'. If there is you need a further
primitive

-   $\operatorname{Temp-less}xy$ meaning the temperature at point $x$ is
    less than at $y$.

The question of whether this primitive makes sense, for any givin
quantity (in this case temperature), may turn on whether the laws are
invariant under replacing uniformly high values of the quantity with low
values. We'll discuss what this means in the case of gravitational
potential below.

Questions

-   Is there a problem of scale for Field? Why not?

-   Can we define the temperature at $x$ is twice the temperature at
    $y$? (Answer: no. why not?)

-   Define temp at $x$ = temp at $y$. (answer:
    $\operatorname{TCong} xyxx$).

-   Can you define the temperature at $x$ is the temperature at $y$ +
    the temperature at $z$. (No: it depends on the choice of 0 -- if you
    move it down by $\epsilon$ $t(y)+t(z)$ increase by $2\epsilon$
    whereas $x$ increases by $\epsilon$.

-   This question illustrates the need for the continuity assumption of
    fields.

    Suppose we define absolute 0 to be the temperature at a point $u$.
    Define the idea that the temp at $x$ is the sum of $y$ and $z$ in
    terms of $u$. (Ans: you need the continuity of fields. There exists
    a point $w$ whose temp is between $u$ and $x$ such that $uw$ is
    congruent to $uy$ and $wx$ is congruent to $uz$.)

-   Can you define the temperature at $x$ is 1 (we don't have units).
    Use this to explain why we can't define the idea that the
    temperature at $x$ is the product of the temperatures at $z$ and
    $w$, even relative to a choice of $0$. What about relative to a
    choice of unit?

-   Suppose that you're Newton, and there is a single three dimensional
    space. What issues would arise if we took a four-place TCong
    relation and a three-place TBet relation on points of space as our
    primitive? (Think about what would happen if the temperature was
    uniformly increasing over time, without.)

-   What would be a better set of primitives in this setting? (Ans: a
    five-place and four-place version of these that have an extra
    parameter for a time.)

Here we outline, in brief, Field's nominalistic version of Newtonian
physics. Roughly speaking, Field's version of Newtonian physics stands
to the platonistic theory as Euclidean geometry (in terms of congruence
and betweenness) stands to platonistic geometry.

-   $GCong\, xyzw$: a relation between points (spacetime events) the
    difference between the gravitational potential at $x$ and $y$ is the
    same as the difference between the gravitational potential at $z$
    and $w$.

-   $GBet\, xyz$ similarly, the gravitaitonal potential at $y$ is
    between it at $x$ and $z$.

## The nominalistic approach to (conservative) vector fields

Recall that we can represent a vector field by the 'slope' of a scalar
field. For instance the gravitational field is the slope of the
gravitational potential.

Questions:

-   Can we define the direction of the gravitational field at point $x$?

How we remove gauge symmetries

-   Lifting and lowering the terrain keeps the relative differences the
    same.

-   This primitive is thus better that

# Relationism and the problem of numbers and scale

Suppose you're a relationist. You don't believe in regions, but you do
believe in material objects. Note that while we originally conceived of
geometry as a theory of space, the relationist can still make sense of
geometrical properties: some material objects are spherical, others are
cubes, physical rods can meet at right angles, and so on.

-   For every geometric property of regions the substantivalist believes
    in, there is a corresponding geometry property of material objects.

-   The substantivalist can define this corresponding property from
    their primitives

    -   Example Qu: Define the property of being a ball shaped material
        object using the substantivalists primitives (you may assume
        ball shaped region has been defined, and you have a location
        relation).

-   The relationist, by contrast, only believes in these properties of
    material objects ad does not believe they can be defined.

How, then, should you do geometry if you're a relationist? Note that we
don't have points of space (or spacetime events), so what would be the
relations be between? One way to resolve this issue is to assume that
matter is made up of points of matter that are not themselves composed
of smaller bit of matter. So to do geometry we now talk about points of
matter instead of points of space or spacetime points.

Two options:

-   Platonistic geometry: there is a fundamental relation $D$ relating
    two points of matter to a real number, the distance between them.

-   Monadicism: there is a primitive property of being located at $p$
    for every point the substantivalist recognizes. (Higher-order
    version. But still there's a version of the shift argument.)

-   Nominalistic geometry (Euclid-Tarski style): there are fundamental
    congruence and betweenness primitives relating points of matter.

A useful exercise: recall that in the usual setting substantivalist
setting, can paraphrase away reference to numbers using congruence and
betweenness.

-   The length of $xy$ is three times the length of $zw$: there exists
    $u_1,u_2$ between $x$ and $y$ such that $xu_1$, $u_1u_2$, $u_2y$ and
    $zw$ are all congruent.

-   It's easy to see how to paraphrase away reference to all rational
    numbers this way, and certain reals as well.

How would this work for the relationist setting, where the relation is
between points of matter?

-   Give an example where $xyzw$ fail to satisfy the condition for $xy$
    being twice the length of $zw$, even when $xy$ really is twice the
    length of $zw$.

-   What about other primitives? Take Tarski's definition on touching in
    terms of two spheres?

What are the options?

-   Infinitely many primitives?

-   What about infinitely many

Relative locations:

-   

[^1]: *History of Western Philosophy* p203.

[^2]: Different editions of the Elements differ on whether this
    principle is included.

[^3]: The distance $p$ and $q$ is $\log\frac{|aq||bp|}{|ap|qb|}$ where
    $a$ and $b$ are the points of the boundary of the disc that the arc
    connecting $p$ and $q$ intersect, and $|cd|$ is the length of that
    arc in the normal sense of length.

[^4]: This last axiom tells us that by rotating a plane about $xy$.

[^5]: This axiom ensures that two triangles $xyz$ and $xyz'$ in the same
    plane have a coordinated right-side. By applying this axiom three
    times we can ensure that *any* three triangles $xyz$ and $x'y'z'$ in
    the same plane, labelled in the same direction, agree about what is
    right. (Note: this actually makes the second axiom redundant).

[^6]: Ibn Sina, however, thought that impetus required air resistance to
    dissipate, and thus a body with impetus and with no other forces
    action on it would travel with constant speed, partially
    anticipating Newton's first law.

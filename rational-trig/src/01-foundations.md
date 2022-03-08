# Foundations

We will look at the foundational knowledge and assumptions that will underlie
our exploration of triangles and their uses. We will also define some of the
basic tools. 

##  Distance

Distance is our starting point. This already is based on a lot of structure
and assumptions, but distance is something generally familiar in the real
world and it is our gateway of correspondence. It also provides us with the
basic external tool we need for constructing the rest. 

Line segments are intimately connected with distance. We are basically
assuming we can assign line segments numbers such that when two line segments
line up, they have the same number, when we have multiple copies of a line
segment joined up in a "line", then the distance is that multiple from one
side to the other. 

Distance is the assignment to two points a number and that assignment has some
nice properties: 

* Our distance will be non-negative and is 0 exactly when the two points are the same
  point. 
* If we have points A, B, and C, then d(A,B) plus d(B,C) will be greater than
  the d(A,C) unless A, B, and C are all on the same line in which case the sum
  is equal to d(A,C), assuming d(A,C) is the larger of the three. This is
  somewhat the definition of a line. 
* ...

## Lines

Two points define a line by the addition property above, namely any third
point is on the line precisely when there is an arrangement of the distance
sum such that the third pair is equal to the sum. It is equivalent to
saying that all three line segments defined by each pair of the three points
overlap one another. This assume line segments are defined which can be said
to be the shortest distance between two points, but that assumes being able to
apply our distance notion to generate lengths of paths and also the definition
of paths. 

We take this as our foundation and have already pointed out some of the
foundational issues in trying to make a cleaner base. We take the attitude
that we are applying this in the real world and that the notion of line
segments and distances from those segments are well understood. 

Given two lines, they will either intersect at one point, are the same line,
or do not intersect at all. If they do not intersect, we call them parallel
lines. They essentially go in the same direction as one another, somewhat a
notion defined in terms of parallelity. 

If lines intersect at one point, then they form four angles. Pairs of opposing
angles can be rotated onto one another, that is they are congruent. If all
four angles are congruent, then that is a right angle. Lines that intersect in
such a way are called perpendicular lines. 

The exploration of the intersection is most easily done with coordinates as we
will discuss later. 

## Triangles

We define triangles to be the figures formed from joining the three line
segments defined by three non-collinear points. Much of work will be exploring
triangles and there uses. 

Each of the three points are called vertices. The three line segments are the
sides. At the segment joins, we get angles. Three of them for the interior of
the triangle. 

## Circles

After lines, circles are the next structure to define as it allows us to define 
right angles. 

A point is on a circle with a given center and radius exactly when the
distance from the point to the center is the radius. It consists of the points
equidistant to the center with that common distance being the radius. 

Two circles will generally intersect in no points (one is wholly inside the
other or they are separated sufficiently far from one another), intersect in
one point (they just touch one another, the centers are exactly the distance
of the two radii added together), intersect in two points, or are the same
circle. 

Finding the intersections is generally best done in coordinates and involves
solving quadratic equations that happen to generally have 0, 1, 2, or
infinitely many solutions. 

One particular circular construction of relevance for us is the construction
of perpendicular angles. This is done as follows: 

1. Draw a line segment.
2. Draw two circles. Each circle should have one endpoint as the center and
   have radius equal to the line segment. Very symmetrical.
3. Find the intersection of the two circles. This will consist of two points.
4. Draw in the line segment between these two points. 
5. The original line segment and the new line segment will intersect at the
   midpoint of each segment and meet at a right angle. This is from symmetry.
6. If the square of the length of the original line segment is 1, then the
   square of the new line segment is 3/2. This relies on the Pythagorean
   theorem talked about later. 
7. Connecting the two centers and one of the intersection points will form an
   equilateral triangle. This is by definition of the point of intersection
   being on each circle. 
8. Any segments formed from joining the centers to a given point on this perpendicular bisector will be equal. This is from symmetry. 

The symmetry argument follows from imagining flipping the picture around or
flipping it up and down. There should be no difference and thus the segments
must be equal and the angles congruent. 

This construction relies very much on the existence of the intersection
points. In a coordinate based solution, the coordinates will involve
irrational numbers. The existence of the intersection therefore depends on the
existence of irrational numbers and is non-trivial. 

To get perpendiculars without irrational numbers, draw two circles with
centers at the endpoints but that just touch, that is, they intersect at
just one point. That point will be the midpoint (by symmetry), and the unique
line that intersects the circles at exactly that point will be perpendicular
to the line segment. 


## Area

We start by defining areas of rectangles. Rectangles are four-sided figures
with each angle being a right angle. 

When we stack rectangles next to each other, our notion of area combines those
rectangles in a fashion linearly related to the sides being combined. For
example, placing a copy of a rectangle next to each other produces another rectangle
with one of the pair of opposite side lengths doubled and the area also doubled. Do this
repeatedly to get a full rectangle with both sides doubled and the area ends
up being quadrupled. If we did this such that each side was tripled, we would
get 9 original rectangles and 9 times the area. 

By working that out, we realize the formula for area is  Length\*Width\*fundamental unit
area. We will ignore the fundamental unit area in formulas, but it is very
important to understand that it is there and is why we say things like square
feet. 

We have therefore defined the area of rectangles. We can then build that for
defining other areas by tiling them with rectangles or making rectangles out
of them. 

This latter strategy is how we derive the triangle area. We start with right
triangles, that is, a triangle where two sides meet at a right angle. The side
opposite the right angle is the hypotenuse. 

Given a right triangle, we can construct a rectangle by flipping it across the
hypotenuse. The length and width of the triangle, generally called base and
height, becomes that of the rectangle. We know the rectangle's area is
base*height and since there were two triangles, the area of each triangle is
half that of the rectangle. So b\*h/2. 

For general triangles, we pick a vertex and drop the perpendicular to the
opposite side. The length of that segment is the height. The base is the
length of the opposite side. The area is then b\*h/2.  

To see that, we need two cases. If the perpendicular is within the original
triangle, we get two right triangles whose areas sum to the original. They
have the same height, but they split the base. So the sum of the areas will
restore that base length. This is case that happens when all the angles in the
triangle are acute or we use the obtuse angle in an obtuse triangle. 

The
second case is when we use an acute angle in an obtuse triangle. Here the
perpendicular goes outside the triangle. We form two new right triangles from
this, one larger than the original and one smaller than the original. If we
subtract the smaller from the original, we get the original area. This will
subtract the extra bit on the base. 

## Pythagorean Theorem

This is a pretty essential theorem.  It has hundreds of proofs and many
applications. 

Given a right triangle, the sum of the square of the two legs (smaller sides, they form the
right angle), will be equal to the square of the hypotenuse (side opposite
right angle).  

The proof here is a bit algebraic and a bit geometric. Given right triangle
with side lengths a, b, and hypotenuse length c, form the square with side lengths a+b. Inside
the rectangle draw four copies of the original right triangle, one for each
right angle in the rectangle. This forms a square inside with side length c.
The rectangle area is therefore both $(a+b)^2 = a^2 + 2ab + b^2$ as well as 
$4* \tfrac{ab}{2} + c^2$ which leads to $a^2 + b^2 = c^2$. 

We will employ the term quadrance for the length squared. If P, Q, and R are
the squares of the side lengths a, b, and c,  then the Pythagorean Theorem can
be stated as  P + Q = R.  

## Angles

When two lines meet, they form four angles, generally two distinct angles (not
congruent). 

A large portion of what we will be concerned with is the measure of an angle.
It is a way of representing the essential feature of the angle, just as
distance is an essential feature of representing a line segment. 

We will have two different notions of measures of angles. The classical notion
is a linearization of the measure of an angle so that we can add the measure
of adjacent angles together. This is a very nice feature. 

The other notion of a measure of angle is to tie it to a canonical
representation using right triangles. Essentially, we represent the angle
embedded in a right triangle and we can summarize that right triangle in a
single number. There are multiple representations one can choose, but we will
primarily use what is called spread.  

### Linear Angle Measure

We can attempt to measure this directly by drawing a circle whose center is
the vertex of the angle. It will be cut by the two lines into four arcs,
with opposing arcs being congruent. An angle is a right angle exactly when all four arcs are
congruent to one another. If it is not a right angle, there is a smaller arc
and a larger arc whose combination will be half the circle.  The smaller angle
is called an acute angle and the larger is an obtuse angle. 

To get a measure, we need to measure the length of the arc as a fraction of
the total circle length and scale it appropriately. To do the straightforward
fraction taking, we call that a turn measure (wildberger), and it has the
property that 1 is a full rotation around the circle, and a 1/4 is a right
angle. 

We convert from the Turn measure to standard degrees by multiplying by 360
degrees. There is also a European standard of gradians in which we scale by
multiplying by 400. The primary mathematical measure used is that of radians.
For this we multiply by $2\pi$. This latter measure has the distinct
unpleasantness of any decimal representation having to be an approximate form.
The main advantage of radians is that the trigonometric functions have
particularly nice properties. 

If we use these measures, then two adjacent angles have the property that the
sum of their measures is the measure of the outside angle combining them. This
is useful, but it does come at the price of imprecise measuring of angles
since we can't really linearize the circular measure. Most of our measurements
of angles actually come from inverting the trigonometric functions and
measuring lengths.   (Is this really true)


## Spread Measure

Our alternate angle measurement is based on the idea of representing an angle
with a right triangle. The basic thesis, which we will establish, 






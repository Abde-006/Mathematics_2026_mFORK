# Solution 13 - Intersection of a Sphere and a Plane

## Problem statement

Given the sphere

$$
x^2+y^2+z^2=25
$$

and the plane $z=3$, find the equation of the intersection curve and its radius. Then describe the behavior for $z=c$.

## Lettered quantities

- Let $R=5$ denote the sphere radius and $c$ the plane height.

## Step 1 - Substitute $z=3$

**Sphere-plane section formula.** Substituting $z=c$ in $x^2+y^2+z^2=R^2$ gives $x^2+y^2=R^2-c^2$; real points require $R^2-c^2\ge0$. Apply $R=5,c=3$:
 $z=3$

The plane equation requires $z=3$ at every point of the intersection. Substitute into the sphere:

$$
x^2+y^2+3^2=25.
$$

Subtract $9$:

$$
x^2+y^2=16.
$$

Together with $z=3$, this is

$$
x^2+y^2=16,\qquad z=3.
$$

Therefore the intersection is a circle centered at $(0,0,3)$ with radius

$$
r=\sqrt{16}=4.
$$

## Step 2 - Analyze $z=c$

**General fixed-height reminder.** The same section equation applies for any $c$:
 the general height $z=c$

Substitute $z=c$:

$$
x^2+y^2+c^2=25,
$$

so

$$
x^2+y^2=25-c^2.
$$

The section is a circle of radius $\sqrt{25-c^2}$ when $|c|<5$. It is the point $(0,0,c)$ when $|c|=5$. It is empty when $|c|>5$.

At $c=5$ the point is $(0,0,5)$, and at $c=-5$ it is $(0,0,-5)$.

## Verification

For a point in the intersection at $z=3$,

$$
x^2+y^2+z^2=16+9=25.
$$

This independently confirms every point on $x^2+y^2=16$ lies on the sphere.

An alternative geometric calculation uses the right triangle formed by the sphere radius $R=5$, the center-to-plane distance $3$, and the intersection radius $r$:

$$
r^2+3^2=5^2,
$$

so

$$
r^2=25-9=16,\qquad r=4.
$$

## Geometric interpretation

Horizontal sections are largest in the plane $z=0$, where $r=5$, and shrink as $|c|$ approaches $5$. The planes $z=\pm5$ meet the sphere only at the north and south poles.

## Final answer

The intersection with $z=3$ is

$$
x^2+y^2=16,\qquad z=3,
$$

a circle of radius $4$. For height $z=c$, the radius is $\sqrt{25-c^2}$ when $|c|<5$, with point sections at $c=\pm5$ and no real section outside that range.

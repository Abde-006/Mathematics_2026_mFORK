# Solution 13 — Intersection of a Sphere and a Plane

## Problem Statement

Find the intersection of the sphere $x^2+y^2+z^2=25$ with the plane $z=3$ and give its radius. Describe the sections at $z=c$ for all values of $c$.

## Objective

Find planar sections of a sphere by substituting the fixed coordinate.

## Concepts and Formulas

A sphere centered at the origin with radius $R$ has equation $x^2+y^2+z^2=R^2$. At height $z=c$, the section satisfies $x^2+y^2=R^2-c^2$.

## Step-by-Step Solution

Substitute $z=3$:

$$
x^2+y^2+3^2=25,
\qquad
x^2+y^2=16.
$$

The intersection is a circle centered at $(0,0,3)$ within the plane $z=3$, with radius $4$.

For a general height $z=c$:

$$
x^2+y^2=25-c^2.
$$

If $|c|<5$, the section is a circle of radius $\sqrt{25-c^2}$. At $c=5$ or $c=-5$, it is one point, respectively $(0,0,5)$ or $(0,0,-5)$. For $|c|>5$, there is no real intersection. The circles are largest at $c=0$ and shrink toward the two poles.

## Verification

Every point on the intersection circle has $x^2+y^2=16$ and $z^2=9$, so $x^2+y^2+z^2=16+9=25$. Its radius $4$ also follows from the right triangle with sphere radius $5$ and center-to-plane distance $3$: $4^2+3^2=5^2$.

## Final Answer

The intersection at $z=3$ is

$$
x^2+y^2=16,\qquad z=3,
$$

a circle of radius $4$. At height $z=c$, the radius is $\sqrt{25-c^2}$ for $|c|<5$; the sections reduce to points at $c=\pm5$ and are empty for $|c|>5$.

## Key Takeaways

- Substituting the plane equation directly gives the intersection curve.
- The sphere's horizontal sections shrink to points at its top and bottom.
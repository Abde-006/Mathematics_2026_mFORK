# Solution 8 — Sphere

## Problem Statement

Reduce

$$
x^2+y^2+z^2-4x+2y-6z-2=0
$$

to canonical form, find the center and radius, and verify two points on the sphere.

## Objective

Extend completing the square from circles to three-dimensional spheres.

## Concepts and Formulas

A sphere with center $(h,k,\ell)$ and radius $r$ has equation $(x-h)^2+(y-k)^2+(z-\ell)^2=r^2$.

## Step-by-Step Solution

Group the terms and move the constant:

$$
(x^2-4x)+(y^2+2y)+(z^2-6z)=2.
$$

Complete each square, adding $4$, $1$, and $9$ to both sides:

$$
(x^2-4x+4)+(y^2+2y+1)+(z^2-6z+9)=2+4+1+9.
$$

Therefore

$$
(x-2)^2+(y+1)^2+(z-3)^2=16.
$$

The center is $(2,-1,3)$ and the radius is $4$.

Take points four units from the center along the positive $x$- and $y$-directions: $(6,-1,3)$ and $(2,3,3)$. Each has squared distance $16$ from the center. In the original left-hand side, their values are, respectively,

$$
36+1+9-24-2-18-2=0,
$$

$$
4+9+9-8+6-18-2=0.
$$

## Verification

Expanding the canonical equation gives $x^2+y^2+z^2-4x+2y-6z-2=0$. Both selected points satisfy it directly and have distance $4$ from the center.

## Final Answer

$$
(x-2)^2+(y+1)^2+(z-3)^2=16
$$

The sphere has center $(2,-1,3)$ and radius $4$.

## Key Takeaways

- Complete one square for each coordinate.
- The radius squared is the final right-hand side after all square constants are added.
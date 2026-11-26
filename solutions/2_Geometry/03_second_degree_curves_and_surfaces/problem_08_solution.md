# Solution 8 - Sphere

## Problem statement

Reduce

$$
x^2+y^2+z^2-4x+2y-6z-2=0
$$

to canonical form. Find the center and radius, give two points on the sphere, and check them.

## Lettered quantities

- Let $(h,k,\ell)$ denote the sphere center and $r>0$ its radius.

## Step 1 - Group

**Sphere completing-square property.** Complete each variable using $u^2+bu=(u+b/2)^2-(b/2)^2$, because the result becomes a sum of squared distances from $(h,k,\ell)$. Group:

Group by coordinate:

$$
(x^2-4x)+(y^2+2y)+(z^2-6z)=2.
$$

## Step 2 - Complete

**Apply the square completion.** Complete $x,y,z$ separately, preserving the constants on the right:
 each square

The completing-square constants are

$$
\left(\frac{-4}{2}\right)^2=4,\qquad
\left(\frac2{2}\right)^2=1,\qquad
\left(\frac{-6}{2}\right)^2=9.
$$

Add $4$, $1$, and $9$ to both sides:

$$
(x^2-4x+4)+(y^2+2y+1)+(z^2-6z+9)=2+4+1+9.
$$

Factor each square:

$$
(x-2)^2+(y+1)^2+(z-3)^2=16.
$$

## Step 3 - Read

**Sphere form.** $(x-h)^2+(y-k)^2+(z-\ell)^2=r^2$ has center $(h,k,\ell)$ and radius $r$. Compare:
 the center and radius

Comparing with $(x-h)^2+(y-k)^2+(z-\ell)^2=r^2$ gives

$$
(h,k,\ell)=(2,-1,3),\qquad r=\sqrt{16}=4.
$$

## Step 4 - Check

**Point-on-sphere test.** A point lies on the sphere exactly when substitution gives $r^2$. Choose and test two points:
 two points

Move $r=4$ from the center in the positive $x$ direction and positive $y$ direction. The resulting points are

$$
P=(6,-1,3),\qquad Q=(2,3,3).
$$

In the canonical form,

$$
(6-2)^2+(-1+1)^2+(3-3)^2=16,
$$

and

$$
(2-2)^2+(3+1)^2+(3-3)^2=16.
$$

In the original left-hand side,

$$
L(P)=36+1+9-24-2-18-2=0,
$$

and

$$
L(Q)=4+9+9-8+6-18-2=0.
$$

## Verification

Expanding the canonical equation gives

$$
x^2+y^2+z^2-4x+2y-6z-2=0,
$$

so no algebraic step was lost in completing the squares.

## Geometric interpretation

The sphere is centered at $(2,-1,3)$ and has radius $4$. It reaches four units in every coordinate direction from its center.

## Final answer

The canonical equation is

$$
(x-2)^2+(y+1)^2+(z-3)^2=16.
$$

The center is $(2,-1,3)$ and the radius is $4$. Two points on the sphere are $(6,-1,3)$ and $(2,3,3)$.

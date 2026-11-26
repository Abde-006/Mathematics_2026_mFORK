# Solution 2 - Circle by Completing the Square

## Problem statement

Reduce

$$
x^2+y^2-6x+4y-3=0
$$

to canonical form. Find the center and radius, then substitute two points from the circle into both forms.

## Lettered quantities

- Let $(h,k)$ denote the circle center and let $r>0$ denote the radius.

## Step 1 - Group

**Completing-the-square property.** $u^2+bu=(u+b/2)^2-(b/2)^2$ removes the linear term while preserving the quadratic value. Group using

Regroup by variable:

$$
(x^2-6x)+(y^2+4y)=3.
$$

## Step 2 - Complete

**Apply the square reminder.** For $u=x$ or $y$, add and subtract $(b/2)^2$ inside each grouped expression:
 both squares

For $x^2-6x$, $b=-6$, so $(b/2)^2=(-3)^2=9$. For $y^2+4y$, $b=4$, so $(b/2)^2=2^2=4$.

Add $9$ and $4$ to both sides:

$$
(x^2-6x+9)+(y^2+4y+4)=3+9+4.
$$

The first square factorization gives $(x-3)^2$, and the second gives $(y+2)^2$. Therefore

$$
(x-3)^2+(y+2)^2=16.
$$

Thus $h=3$, $k=-2$, and $r^2=16$, so $r=4$.

## Step 3 - Choose

**Circle recognition.** Once the equation is $(x-h)^2+(y-k)^2=r^2$, $(h,k)$ is the center and $r$ is the radius. Rewrite and choose points:

Choose $P=(7,-2)$ and $Q=(3,2)$, obtained by moving $r=4$ from the center horizontally and vertically.

In the canonical form,

$$
(7-3)^2+(-2+2)^2=4^2+0=16,
$$

and

$$
(3-3)^2+(2+2)^2=0+4^2=16.
$$

In the original left-hand side,

$$
7^2+(-2)^2-6(7)+4(-2)-3
=49+4-42-8-3=0,
$$

and

$$
3^2+2^2-6(3)+4(2)-3
=9+4-18+8-3=0.
$$

## Verification

Expanding the canonical form gives

$$
x^2-6x+9+y^2+4y+4=16,
$$

which simplifies to

$$
x^2+y^2-6x+4y-3=0.
$$

Thus the two forms describe exactly the same circle.

## Geometric interpretation

The factor $(x-3)^2$ locates the center three units to the right of the origin, while $(y+2)^2$ locates it two units below the origin.

## Final answer

The canonical equation is

$$
(x-3)^2+(y+2)^2=16.
$$

The circle has center $(3,-2)$ and radius $4$. Both $(7,-2)$ and $(3,2)$ satisfy both forms.

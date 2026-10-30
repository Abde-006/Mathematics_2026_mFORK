# Solution 2 — Circle by Completing the Square

## Problem Statement

Reduce

$$
x^2+y^2-6x+4y-3=0
$$

to canonical form, find the center and radius, and check two points in both forms.

## Objective

Complete the square in each variable to reveal the circle's center and radius.

## Concepts and Formulas

For a quadratic expression $u^2+bu$, add and subtract $(b/2)^2$ to obtain $(u+b/2)^2-(b/2)^2$. A circle in canonical form is $(x-h)^2+(y-k)^2=r^2$.

## Step-by-Step Solution

Group the terms in each variable and move the constant:

$$
(x^2-6x)+(y^2+4y)=3.
$$

Complete each square:

$$
(x^2-6x+9)+(y^2+4y+4)=3+9+4.
$$

Thus

$$
(x-3)^2+(y+2)^2=16.
$$

The center is $(3,-2)$ and the radius is $4$.

Choose the points $(7,-2)$ and $(3,2)$, each four units from the center. In canonical form, each gives $4^2+0^2=16$. In the original left-hand side:

$$
7^2+(-2)^2-6(7)+4(-2)-3=49+4-42-8-3=0,
$$

$$
3^2+2^2-6(3)+4(2)-3=9+4-18+8-3=0.
$$

## Verification

Expanding the canonical equation gives $x^2-6x+9+y^2+4y+4=16$, which simplifies to the original equation. Both selected points satisfy both forms.

## Final Answer

$$
(x-3)^2+(y+2)^2=16
$$

The circle has center $(3,-2)$ and radius $4$.

## Key Takeaways

- The completed-square constants must be added to both sides.
- The signs inside the factors locate the center: $(x-3)^2$ gives $x=3$, and $(y+2)^2$ gives $y=-2$.
# Solution 6 — Shifted Ellipse

## Problem Statement

Reduce

$$
4x^2+9y^2-16x+18y-11=0
$$

to canonical form, find the center and semiaxis lengths, and check the original left-hand side at the center.

## Objective

Complete the square while accounting for the coefficients of the quadratic terms.

## Concepts and Formulas

Factor the coefficient of each squared variable before completing its square. The ellipse $(x-h)^2/a^2+(y-k)^2/b^2=1$ has center $(h,k)$ and semiaxes $a,b$.

## Step-by-Step Solution

Group and factor:

$$
4(x^2-4x)+9(y^2+2y)-11=0.
$$

Complete the squares inside the parentheses. Since $(-4/2)^2=4$ and $(2/2)^2=1$, add $4(4)$ and $9(1)$ to the left side and to the right side:

$$
4\bigl((x-2)^2-4\bigr)+9\bigl((y+1)^2-1\bigr)-11=0.
$$

Collect the constants:

$$
4(x-2)^2+9(y+1)^2=36.
$$

Divide by $36$:

$$
\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1.
$$

The center is $(2,-1)$. The semiaxis lengths are $3$ along the $x$-direction and $2$ along the $y$-direction.

At the center, the original left-hand side is

$$
4(2)^2+9(-1)^2-16(2)+18(-1)-11=16+9-32-18-11=-36.
$$

This agrees with the unnormalized completed equation, whose left side at the center is $0+0-36=-36$.

## Verification

Expanding $4(x-2)^2+9(y+1)^2=36$ gives $4x^2+9y^2-16x+18y-11=0$. The center check also matches the constant shift.

## Final Answer

$$
\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1
$$

The curve is an ellipse centered at $(2,-1)$ with semiaxes $3$ and $2$.

## Key Takeaways

- Keep each quadratic coefficient outside its parentheses while completing the square.
- Divide by the right-hand constant to read the semiaxis lengths.
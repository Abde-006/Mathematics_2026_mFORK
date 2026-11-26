# Solution 6 - Shifted Ellipse

## Problem statement

Reduce

$$
4x^2+9y^2-16x+18y-11=0
$$

to canonical form. Give the center and semiaxis lengths, and check the left-hand side at the center.

## Lettered quantities

- Let $(h,k)$ denote the ellipse center and let $a,b>0$ denote its semiaxes.

## Step 1 - Factor

**Completing-the-square preparation.** Factor each quadratic coefficient before completing each square, so the linear coefficients remain associated with their variables:

Factor the quadratic coefficients:

$$
4(x^2-4x)+9(y^2+2y)-11=0.
$$

## Step 2 - Complete

**Square-completion reminder.** $u^2+bu=(u+b/2)^2-(b/2)^2$. Apply separately to $x$ and $y$:
 both squares

Inside the $x$ parentheses, $(-4/2)^2=4$. Inside the $y$ parentheses, $(2/2)^2=1$. Therefore

$$
4\bigl((x-2)^2-4\bigr)+9\bigl((y+1)^2-1\bigr)-11=0.
$$

Expanding the subtracted constants gives

$$
4(x-2)^2-16+9(y+1)^2-9-11=0.
$$

Combine the constants and move them to the right:

$$
4(x-2)^2+9(y+1)^2=36.
$$

## Step 3 - Normalize

**Canonical ellipse form.** $(x-h)^2/a^2+(y-k)^2/b^2=1$ identifies $(h,k)$ and the semiaxes $a,b$. Divide and compare:


Divide every term by $36$:

$$
\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1.
$$

Comparing with the canonical formula gives $h=2$, $k=-1$, $a^2=9$, and $b^2=4$. Therefore

$$
(h,k)=(2,-1),\qquad a=3,\qquad b=2.
$$

## Step 4 - Check

**Center substitution.** At $(h,k)$ the translated squared terms vanish. Substitute $(h,k)$ into the original left-hand side to verify consistency:
 the center

Substitute $(x,y)=(2,-1)$ into the original left-hand side:

$$
\begin{aligned}
L(2,-1)
&=4(2)^2+9(-1)^2-16(2)+18(-1)-11 \\
&=16+9-32-18-11 \\
&=-36.
\end{aligned}
$$

This is consistent with the unnormalized completed equation: at the center,

$$
4(0)^2+9(0)^2-36=-36.
$$

## Verification

Expanding the canonical form,

$$
4(x-2)^2+9(y+1)^2=36,
$$

returns

$$
4x^2-16x+16+9y^2+18y+9=36,
$$

and hence

$$
4x^2+9y^2-16x+18y-11=0.
$$

## Geometric interpretation

The ellipse is centered at $(2,-1)$, with horizontal semiaxis $3$ and vertical semiaxis $2$. It is more stretched along the $x$ direction.

## Final answer

The canonical equation is

$$
\frac{(x-2)^2}{9}+\frac{(y+1)^2}{4}=1.
$$

Its center is $(2,-1)$ and its semiaxes are $3$ and $2$.

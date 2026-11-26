# Solution 7 - Classifying a Second-Degree Equation

## Problem statement

Determine the type of object described by:

1. $4x^2+9y^2=36$,
2. $x^2-y^2=1$,
3. $x^2-4y=0$,
4. $x^2+y^2+1=0$.

In the last case, explain why no real point exists.

## Lettered quantities and recognition rules

Let $a,b>0$. Recognition uses these canonical forms:

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

This sign pattern describes an ellipse.

$$
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
$$

This sign pattern describes a horizontal hyperbola.

$$
x^2=4py
$$

This sign pattern describes a parabola.

where $p$ is positive for an upward-opening parabola and negative for a downward-opening one.

## Step 1 - $4x^2+9y^2=36$

Divide by $36$:

$$
\frac{4x^2}{36}+\frac{9y^2}{36}=1,
$$

which is

$$
\frac{x^2}{9}+\frac{y^2}{4}=1.
$$

The equation is an ellipse centered at $(0,0)$ with semiaxes $a=3$ and $b=2$.

## Step 2 - $x^2-y^2=1$

The equation already has the form

$$
\frac{x^2}{1}-\frac{y^2}{1}=1.
$$

It is therefore a hyperbola centered at $(0,0)$ with $a=b=1$. It opens along the $x$-axis and has vertices $(\pm1,0)$.

## Step 3 - $x^2-4y=0$

Rearrange:

$$
x^2=4y.
$$

Comparing with $x^2=4py$ gives $4p=4$, so $p=1$. The object is a parabola with vertex $(0,0)$, axis $y=0$, and upward opening.

## Step 4 - $x^2+y^2+1=0$

Rearrange to

$$
x^2+y^2=-1.
$$

For real $x$ and $y$,

$$
x^2\ge0,\qquad y^2\ge0,
$$

and consequently

$$
x^2+y^2\ge0.
$$

Its smallest possible value is $0$, attained at $(0,0)$, so it can never equal $-1$. Therefore the equation has no real points.

## Verification

The first three equations match canonical conic forms after normalization or rearrangement. The fourth cannot be satisfied because a sum of real squares cannot be negative.

## Final answer

1. An ellipse, $\frac{x^2}{9}+\frac{y^2}{4}=1$.
2. A horizontal hyperbola, $x^2-y^2=1$.
3. An upward-opening parabola, $x^2=4y$.
4. No real curve or set of real points.

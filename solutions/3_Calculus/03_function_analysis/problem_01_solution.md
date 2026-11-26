# Problem 1. A Cubic Polynomial

## Problem

For $f(x)=x^3-3x^2+2$, analyze monotonicity and extrema, and sketch the graph with the critical points marked.

## Solution

Let $f(x)=x^3-3x^2+2$. The first derivative gives the slope.

### Step 1 - Differentiate

The monotonicity test uses the sign of $f'(x)$: a positive derivative means the function is increasing, a negative derivative means decreasing, and a sign change locates an extremum.

$$
f'(x)=3x^2-6x=3x(x-2).
$$

The critical points are $x=0$ and $x=2$.

### Step 2 - Sign chart

Testing between the zeros:

$$
\begin{aligned}
x<0 &: f'(x)>0,\\
0<x<2 &: f'(x)<0,\\
x>2 &: f'(x)>0.
\end{aligned}
$$

Thus $f$ increases on $(-\infty,0)$ and $(2,\infty)$, and decreases on $(0,2)$.

### Step 3 - Values and verification

$$
f(0)=2,\qquad f(2)=8-12+2=-2.
$$

At $x=0$ the derivative changes positive to negative, so $(0,2)$ is a local maximum. At $x=2$ it changes negative to positive, so $(2,-2)$ is a local minimum. The positive leading coefficient is consistent with $f(x)\to-\infty$ as $x\to-\infty$ and $f(x)\to\infty$ as $x\to\infty$.

## Final Answer

Increasing on $(-\infty,0)$ and $(2,\infty)$; decreasing on $(0,2)$; local maximum $(0,2)$; local minimum $(2,-2)$.

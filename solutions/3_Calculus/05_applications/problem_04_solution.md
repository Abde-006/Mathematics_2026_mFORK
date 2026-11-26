# Problem 4. Area Between Curves

Find the area of the region bounded by $y=x$ and $y=x^2$, including the intersection points and the relative position of the curves.

## Quantities

Let $f(x)=x$, $g(x)=x^2$, and $A$ denote the bounded area.

## Step 1 - Find the intersection points

Intersection points satisfy the same $y$-coordinate for both graphs. Thus

$$
\begin{aligned}
x&=x^2, \\
x^2-x&=0, \\
x(x-1)&=0.
\end{aligned}
$$

Hence $x=0$ or $x=1$. The points are $(0,0)$ and $(1,1)$.

## Step 2 - Determine which function is greater

On $0<x<1$, the upper-minus-lower difference is

$$
x-x^2=x(1-x)>0.
$$

Therefore $y=x$ is above $y=x^2$ throughout the bounded interval.

## Step 3 - Compute the area

For an upper function $f$ and lower function $g$ on $a\le x\le b$, the area is

$$
A=\int_a^b(f(x)-g(x)\,)\,dx.
$$

This integral accumulates the vertical height $f-g$ over the interval. Using $f(x)=x$, $g(x)=x^2$, $a=0$, and $b=1$,

$$
\begin{aligned}
A
&=\int_0^1(x-x^2)\,dx \\
&=\left[\frac{x^2}{2}-\frac{x^3}{3}\right]_0^1 \\
&=\left(\frac12-\frac13\right)-0 \\
&=\frac16.
\end{aligned}
$$

## Verification

The result is positive, as required for area. The intersection points determine exactly the interval $[0,1]$, and $x-x^2>0$ confirms the chosen upper and lower functions.

## Interpretation

The bounded region is the crescent-like strip between the line and the parabola, widest near $x=\frac12$ and disappearing at both endpoints.

## Final answer

The area is $\frac16$.

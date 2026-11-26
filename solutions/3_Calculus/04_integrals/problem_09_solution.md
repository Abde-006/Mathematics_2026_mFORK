# Problem 9. Definite Integral and Geometric Area

## Problem

Compute $\int_{-1}^{2}x dx$, then separately find geometric areas below and above the $x$-axis.

## Solution

Let $f(x)=x$. It is negative on $[-1,0)$ and positive on $(0,2]$.

### Exact integral

$$
\int_{-1}^{2}x dx
=\left[\frac{x^2}{2}\right]_{-1}^{2}
=\frac42-\frac12
=\frac32.
$$

### Signed pieces

$$
\int_{-1}^{0}x dx=-\frac12,\qquad
\int_0^2x dx=2.
$$

Thus signed accumulation is $-\frac12+2=\frac32$.

### Geometric area

The lower triangle has area $\frac12(1)(1)=\frac12$, and the upper triangle has area $\frac12(2)(2)=2$. Total geometric area is

$$
\frac12+2=\frac52.
$$

The definite integral is smaller because the negative region is subtracted.

## Final Answer

Definite integral $3/2$; geometric area $5/2$.

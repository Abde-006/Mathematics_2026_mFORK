# Problem 13. An Integral Depending on the Upper Limit

## Problem

Let $F(x)=\int_0^x(t^2+1)dt$. Determine $F(x)$ and $F'(x)$ and interpret the result.

## Solution

$F(x)$ is accumulated area from $0$ to $x$.

### Step 1

The Fundamental Theorem of Calculus states that $F(x)=\int_a^x f(t)\,dt$ differentiates to $F'(x)=f(x)$, because the accumulated area changes at the local height $f(x)$.

$$
\begin{aligned}
F(x)
&=\left[\frac{t^3}{3}+t\right]_0^x\\
&=\frac{x^3}{3}+x.
\end{aligned}
$$

### Step 2

$$
F'(x)=x^2+1.
$$

This equals the integrand at the upper limit. Moving $x$ by a small $h$ adds approximately $(x^2+1)h$ units of area, so the integrand is the local rate of increase of accumulated area.

## Final Answer

$$
F(x)=\frac{x^3}{3}+x,\qquad F'(x)=x^2+1.
$$

# Problem 10. Complete Function Analysis

## Problem

Complete the analysis of $f(x)=x/(x^2+1)$.

## Solution

Let $f(x)=x/(x^2+1)$.

### Domain, symmetry, zero

$x^2+1>0$ for every real $x$, so $D_f=\mathbb R$. Also $f(-x)=-f(x)$, so $f$ is odd. The only zero is $x=0$.

### Limits

$$
\lim_{x\to\pm\infty}\frac{x}{x^2+1}=0,
$$

so $y=0$ is horizontal and there is no vertical asymptote.

### Monotonicity and extrema

$$
f'(x)=\frac{1-x^2}{(x^2+1)^2}.
$$

The denominator is positive. Therefore $f$ increases on $(-1,1)$ and decreases on $(-\infty,-1)\cup(1,\infty)$. Values are

$$
f(-1)=-1/2,\qquad f(1)=1/2.
$$

Thus $(-1,-1/2)$ is a local minimum and $(1,1/2)$ is a local maximum.

### Convexity

$$
f''(x)=\frac{2x(x^2-3)}{(x^2+1)^3}.
$$

Zeros of $f''$ occur at $x=-\sqrt3,0,\sqrt3$. A sign chart gives concavity on $(-\infty,-\sqrt3)\cup(0,\sqrt3)$ and convexity on $(-\sqrt3,0)\cup(\sqrt3,\infty)$. The inflection points are $(0,0)$ and $(\pm\sqrt3,\pm\sqrt3/4)$.

## Final Answer

Odd, domain $\mathbb R$, zero $0$, horizontal asymptote $y=0$, minimum $(-1,-1/2)$, maximum $(1,1/2)$, and inflections $(0,0)$ and $(\pm\sqrt3,\pm\sqrt3/4)$.

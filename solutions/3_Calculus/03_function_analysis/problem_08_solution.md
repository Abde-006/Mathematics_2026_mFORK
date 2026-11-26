# Problem 8. The Second Derivative

## Problem

For $f(x)=x^4-4x^2$, find extrema, convexity/concavity, and inflection points.

## Solution

Let $f(x)=x^4-4x^2$.

### First and second derivatives

$$
f'(x)=4x^3-8x=4x(x^2-2),
$$

$$
f''(x)=12x^2-8.
$$

The critical points are $x=-\sqrt2,0,\sqrt2$. The second derivative gives $f''(0)=-8<0$, so $(0,0)$ is a local maximum, and $f''(\pm\sqrt2)=16>0$, so $(\pm\sqrt2,-4)$ are local minima.

### Convexity

Set $f''(x)=0$:

$$
12x^2-8=0
\quad\Longrightarrow\quad
x=\pm\sqrt{2/3}.
$$

Since $12x^2-8>0$ outside these roots and negative between them, $f$ is convex (upward) on $(-\infty,-\sqrt{2/3})\cup(\sqrt{2/3},\infty)$ and concave (downward) on $(-\sqrt{2/3},\sqrt{2/3})$.

### Inflection points

At $x=\pm\sqrt{2/3}$,

$$
f(x)=\frac49-\frac83=-\frac{20}{9}.
$$

The sign of $f''$ changes at both roots, so both are inflection points.

## Final Answer

Maximum $(0,0)$; minima $(\pm\sqrt2,-4)$; inflection points $(\pm\sqrt{2/3},-20/9)$.
